---
title: Exchange で EWS を使用してフォルダーを同期させる
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d3bbacd1-8e4b-4fd0-8d27-4cbbc045ec3f
description: クライアントを同期させるために、EWS マネージ API または EWS を使用して、フォルダーの一覧、または変更されたフォルダーの一覧を取得する方法について説明します。
ms.openlocfilehash: 4b0686134d642da34b2890a0e692e3d03e4a9fb1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759066"
---
# <a name="synchronize-folders-by-using-ews-in-exchange"></a>Exchange で EWS を使用してフォルダーを同期させる

クライアントを同期させるために、EWS マネージ API または EWS を使用して、フォルダーの一覧、または変更されたフォルダーの一覧を取得する方法について説明します。
  
Exchange の EWS では、アイテムの同期とフォルダーの同期を使用して、クライアントとサーバー間でメールボックスのコンテンツを同期します。フォルダー同期では、ルート フォルダーにあるフォルダーの初期一覧が取得され、その後時間の経過とともに、それらのフォルダーに対して行われた変更が取得され、新しいフォルダーも取得されます。
  
EWS マネージ API を使用してフォルダー同期を行う場合は、まず [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) メソッドを使用して[ルート フォルダー内のフォルダーの初期一覧を取得](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma)します。 次に、後続の呼び出し時に _cSyncState_ パラメーターの値を更新して、新しいフォルダーと変更されたフォルダーの一覧を取得します。 
  
EWS を使用してフォルダー同期を行うには、[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) 操作を使用して[ルート フォルダー内のフォルダーの初期一覧](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest)を要求し、応答を解析します。その後ある時点で、[ルート フォルダー内のフォルダーに対する変更を取得](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews)し、応答を解析します。 クライアントは、初期のフォルダーまたは変更されたフォルダーの一覧を受信した後、[ローカルに更新を実行](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)します。 今後いつどのように変更を取得するかは、アプリケーションが使用している[同期デザイン パターン](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns)によって異なります。 
  
## <a name="get-the-list-of-all-folders-or-changed-folders-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してすべてのフォルダーまたは変更されたフォルダーの一覧を取得する
<a name="bk_cesyncinitialewsma"> </a>

次のコード例は、ルート フォルダー内のフォルダーの初期一覧を取得した後、ルート フォルダー内のフォルダーに対して前回の同期後に行われた変更の一覧を取得する方法を示しています。 [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) メソッドへの最初の呼び出し時に、_cSyncState_ 値を null に設定します。 メソッドが完了したら、次の **SyncFolderHierarchy** メソッド呼び出しで使用するために _cSyncState_ 値をローカルに保存します。 最初の呼び出しと後続の呼び出しの両方で、変更がなくなるまで、**SyncFolderHierarchy** メソッドの連続呼び出しを使用して、10 回のバッチ処理でフォルダーが取得されます。 次の例は、_propertySet_ パラメーターを IdOnly に設定して、Exchange データベースの呼び出し回数を減らしています。これは[同期のベスト プラクティス](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)です。 この例では、**service** は有効な **ExchangeService** オブジェクト バインドであり、_cSyncState_ は前の **SyncFolderHierarchy** 呼び出しによって返された同期状態を表すものとします。 
  
```cs
// Get a list of all folders in the mailbox by calling SyncFolderHierarchy.
// The folderId parameter must be set to the root folder to synchronize. 
// The propertySet parameter is set to IdOnly to reduce calls to the Exchange database
// because any additional properties result in additional calls to the Exchange database. 
// The syncState parameter is set to cSyncState, which should be null in the initial call, 
// and should be set to the sync state returned by the previous SyncFolderHierarchy call 
// in subsequent calls.
ChangeCollection<FolderChange> fcc = service.SyncFolderHierarchy(new FolderId(WellKnownFolderName.Root), PropertySet.IdOnly, cSyncState);
// If the count of changes is zero, there are no changes to synchronize.
if (fcc.Count == 0)
{
    Console.WriteLine("There are no folders to synchronize.");
}
// Otherwise, write all the changes included in the response 
// to the console. 
// For the initial synchronization, all the changes will be of type
// ChangeType.Create.
else
{
    foreach (FolderChange fc in fcc)
    {
        Console.WriteLine("ChangeType: " + fc.ChangeType.ToString());
        Console.WriteLine("FolderId: " + fc.FolderId);
        Console.WriteLine("===========");
    }
}
// Save the sync state for use in future SyncFolderItems requests.
// The sync state is used by the server to determine what changes to report
// to the client.
string fSyncState = fcc.SyncState;

```

サーバー上の新しいフォルダーまたは変更されたフォルダーの一覧を取得した後、[クライアント上のフォルダーを作成または更新します](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)。
  
## <a name="get-the-initial-list-of-folders-by-using-ews"></a>EWS を使用してフォルダーの初期一覧を取得する
<a name="bk_cesyncewsrequest"> </a>

次の例は、[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) 操作を使用して初期フォルダー階層を取得するための XML 要求を示しています。 これは、[SyncFolderHierarchy メソッドを使用して初期フォルダーの一覧を取得する](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma)ときに EWS マネージ API が送信する XML 要求でもあります。 [SyncFolderHierarchy](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) 操作の [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) 要素は、これが最初の同期であるために含まれません。 次の例は、[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) 要素を **IdOnly** に設定して、Exchange データベースの呼び出し回数を減らしています。これは[同期のベスト プラクティス](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)です。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

次の例は、サーバーが [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) 操作要求を処理した後に返す XML 応答を示しています。 最初の応答には、すべてのフォルダーで [Create](http://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) 要素が含まれます。最初の同期ではすべてのフォルダーが新規と見なされるからです。 一部の属性と要素の値は、読みやすくするために短くなっています。また、いくつかの **Create** 要素ブロックは、簡潔にするために削除されています。 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                   xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADM="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM="
                            ChangeKey="AQAAABY"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkAD/AAA="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADBh="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            ...
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>
```

サーバー上の新しいフォルダーの一覧を受信した後、[クライアント上にフォルダーを作成](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)します。
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a>EWS を使用して前回の同期以降の変更を取得する
<a name="bk_cesyncrespews"> </a>

次の例は、[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) 操作を使用してルート フォルダー内のフォルダーに対する変更の一覧を取得するための XML 要求を示しています。 これは、[ルート フォルダーに対する変更の一覧を取得する](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma)ときに EWS マネージ API が送信する XML 要求でもあります。 この例では、[SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) 要素の値を前回の応答で返された値に設定しています。 また、この例では、返される追加のプロパティを示すために、デモの目的で [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) 要素を **IdOnly** ではなく **AllProperties** に設定しています。 [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) 要素を **IdOnly** に設定することが、[同期のベスト プラクティス](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)です。 **SyncState** の値は、読みやすくするために短くなっています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
      <m:SyncState>H4sIAA==</m:SyncState>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

次の例は、サーバーがクライアントからの [SyncFolderHierarchy 操作](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)要求を処理した後に返す XML 応答を示しています。 この応答は、前回の同期以降 1 つのフォルダーが更新され、1 つのフォルダーが作成されて、1 つのフォルダーが削除されたことを示しています。 [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) 要素の値、**Id** 属性、および **ChangeKey** 属性は、読みやすくするために短くなっています。 
  
要求に **AllProperties**[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) が含まれていたことを思い出してください。 これは単にデモの目的のためです。 運用環境では、**BaseShape** 要素を **IdOnly** に設定することをお勧めします。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
<h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="745" MinorBuildNumber="21" Version="V2_3" 
           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Update>
              <t:Folder>
                <t:FolderId Id="AAMkADM=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQMkADMzADI1==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Meeting Notes</t:DisplayName>
                <t:TotalCount>3</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:EffectiveRights>
                  <t:CreateAssociated>true</t:CreateAssociated>
                  <t:CreateContents>true</t:CreateContents>
                  <t:CreateHierarchy>true</t:CreateHierarchy>
                  <t:Delete>true</t:Delete>
                  <t:Modify>true</t:Modify>
                  <t:Read>true</t:Read>
                  <t:ViewPrivateItems>true</t:ViewPrivateItems>
                </t:EffectiveRights>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Update>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM=" ChangeKey="AQAAABYAA" />
                <t:ParentFolderId Id="AQMkO67A==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Schedules</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:EffectiveRights>
                  <t:CreateAssociated>true</t:CreateAssociated>
                  <t:CreateContents>true</t:CreateContents>
                  <t:CreateHierarchy>true</t:CreateHierarchy>
                  <t:Delete>true</t:Delete>
                  <t:Modify>true</t:Modify>
                  <t:Read>true</t:Read>
                  <t:ViewPrivateItems>true</t:ViewPrivateItems>
                </t:EffectiveRights>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
            <t:Delete>
              <t:FolderId Id="AAMkAD/AAA=" ChangeKey="AQAAAA==" />
            </t:Delete>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-the-client"></a>クライアントを更新する
<a name="bk_nextsteps"> </a>

EWS マネージ API を使用する場合は、新しいフォルダーまたは変更されたフォルダーの一覧を取得した後、[Folder.Load](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) メソッドを使用して新しいフォルダーまたは変更されたフォルダーのプロパティを取得し、それらのプロパティをローカル値と比較して、クライアント上のフォルダーを更新または作成します。 
  
EWS を使用する場合は、[GetFolder 操作](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)を使用して新しいフォルダーまたは変更されたフォルダーのプロパティを取得して、クライアント上のフォルダーを更新または作成します。 
  
## <a name="see-also"></a>関連項目

- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)   
- [Exchange で EWS を使用してアイテムを同期する](how-to-synchronize-items-by-using-ews-in-exchange.md)   
- [Exchange の EWS での同期に関連するエラーの処理](handling-synchronization-related-errors-in-ews-in-exchange.md)
    

