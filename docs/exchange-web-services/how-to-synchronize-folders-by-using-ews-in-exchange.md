---
title: Exchange EWS を使用してフォルダーを同期します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d3bbacd1-8e4b-4fd0-8d27-4cbbc045ec3f
description: クライアントを同期させるために、EWS マネージ API または EWS を使用して、フォルダーの一覧、または変更されたフォルダーの一覧を取得する方法について説明します。
ms.openlocfilehash: 4b0686134d642da34b2890a0e692e3d03e4a9fb1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759066"
---
# <a name="synchronize-folders-by-using-ews-in-exchange"></a>Exchange EWS を使用してフォルダーを同期します。

クライアントを同期させるために、EWS マネージ API または EWS を使用して、フォルダーの一覧、または変更されたフォルダーの一覧を取得する方法について説明します。
  
Exchange の EWS では、アイテムの同期とフォルダーの同期を使用して、クライアントとサーバー間でメールボックスのコンテンツを同期します。フォルダー同期では、ルート フォルダーにあるフォルダーの初期一覧が取得され、その後時間の経過とともに、それらのフォルダーに対して行われた変更が取得され、新しいフォルダーも取得されます。
  
場合は、EWS マネージ API を使用する最初の[最初にルート フォルダー内のフォルダーのリストを取得する](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx)メソッドを使用して、フォルダーの同期を実行するときです。 後続の呼び出し中に新しいおよび変更されたフォルダーの一覧を取得し、 _cSyncState_パラメーターの値を更新します。 
  
EWS を使用して、フォルダーの同期を実行するには、 [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)オペレーションを使用して[最初にルート フォルダー内のフォルダーのリスト](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest)を要求する、応答を解析して、いくつかの時点で、将来的に[内のフォルダーへの変更を取得ルート](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews)、応答を解析するとします。 クライアントは、初期または変更されたフォルダーの一覧を受信した後、[更新プログラムをローカルになります](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)。 将来的に変更を取得する方法とタイミングは、アプリケーションを使用して[同期設計パターン](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns)によって異なります。 
  
## <a name="get-the-list-of-all-folders-or-changed-folders-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してすべてのフォルダーまたは変更されたフォルダーの一覧を取得する
<a name="bk_cesyncinitialewsma"> </a>

次のコード例では、ルート フォルダー内のフォルダーの最初のリストを取得し、前回の同期以降に発生したルート フォルダー内のフォルダーへの変更の一覧を取得する方法を示します。 [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx)メソッドの最初の呼び出し時に_cSyncState_の値を null に設定します。 メソッドが完了すると、次の**SyncFolderHierarchy**メソッドの呼び出しで使用するには、ローカルで_cSyncState_の値を保存します。 最初の呼び出しとそれ以降の呼び出しの両方でフォルダーが変更になるまで、 **SyncFolderHierarchy**メソッドへの連続呼び出しを使用して、10 のバッチで取得されます。 この例では、[同期のベスト プラクティス](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)は、Exchange のデータベースへの呼び出しを減らすために IdOnly に_プロパティ設定_のパラメーターを設定します。 この例では、**サービス**は有効な**ExchangeService**オブジェクトのバインド、その_cSyncState_は、 **SyncFolderHierarchy**の前回の呼び出しによって返された同期状態を表すと仮定します。 
  
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

した後は、[クライアント上のフォルダーを作成または](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)サーバー上の新しいまたは変更されたフォルダーの一覧を取得します。
  
## <a name="get-the-initial-list-of-folders-by-using-ews"></a>EWS を使用してフォルダーの初期一覧を取得する
<a name="bk_cesyncewsrequest"> </a>

[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)オペレーションを使用して最初のフォルダー階層を取得するのには、XML 要求の例を次に示します。 これは、EWS のマネージ API を送信する場合、XML 要求も[、SyncFolderHierarchy メソッドを使用して、最初のフォルダーの一覧を取得](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma)します。 これは最初の同期であるために、 [SyncFolderHierarchy](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx)操作の[同期状態](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx)の要素は含まれません。 この例では、[同期のベスト プラクティス](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)は、Exchange のデータベースへの呼び出しを減らすために**IdOnly**に[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx)の要素を設定します。
  
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

[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)操作の要求を処理した後に、サーバーによって返される XML 応答の例を次に示します。 最初の応答には、すべてのフォルダーは、初期同期中に新しいと見なされるために、すべてのフォルダー[を作成する](http://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx)要素が含まれます。 読みやすさ、いくつかの属性と要素の値が途中で切り捨てられ、簡潔にするためのいくつか**を作成する**要素のブロックが削除されました。 
  
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

した後は、[クライアント上のフォルダーを作成](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)サーバー上の新しいフォルダーの一覧を取得します。
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a>EWS を使用して前回の同期以降の変更を取得する
<a name="bk_cesyncrespews"> </a>

[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)オペレーションを使用してルート フォルダー内のフォルダーへの変更の一覧を取得するのには XML の要求の例を次に示します。 これは、EWS のマネージ API を送信する場合、XML 要求[のルート フォルダーへの変更の一覧を取得](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma)します。 この例では、[同期状態](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx)の要素の値を前の応答で返される値に設定します。 およびデモンストレーションのために次の使用例は返される追加のプロパティを表示するのには**IdOnly**ではなく**AllProperties**に[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx)の要素を設定します。 [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx)の要素を**IdOnly**に設定は、[同期のベスト プラクティス](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)です。 **同期状態**の値が小さすぎると読みやすくするためです。 
  
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

クライアントから[SyncFolderHierarchy 操作](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)の要求を処理した後に、サーバーによって返される XML 応答の例を次に示します。 この応答は、1 つのフォルダーが更新されたこと、1 つのフォルダーが作成された、および 1 つのフォルダーが前回の同期後に削除されましたを示します。 [同期状態](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx)の要素、 **Id**属性、および属性の**変更キー**の値は、読みやすくするために短縮されています。 
  
[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx)の**AllProperties**が要求に含まれていることに注意してください。 これは、デモンストレーションの目的のためだけです。 運用環境で、 **IdOnly**に**BaseShape**の要素を設定することをお勧めします。 
  
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

新規または変更されたフォルダーの一覧を取得、 [Folder.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx)メソッドを使用して、新規または変更されたアイテムのプロパティを取得、ローカルの値にプロパティを比較および更新またはクライアント上でフォルダーを作成した後は、EWS のマネージ API を使用しています。 場合、 
  
EWS を使用する場合は、新規または変更されたフォルダーのプロパティを取得、更新、またはクライアント上でフォルダーを作成する[GetFolder の操作](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)を使用します。 
  
## <a name="see-also"></a>関連項目

- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)   
- [Exchange EWS を使用して項目を同期します。](how-to-synchronize-items-by-using-ews-in-exchange.md)   
- [Exchange EWS での同期に関連するエラーの処理](handling-synchronization-related-errors-in-ews-in-exchange.md)
    

