---
title: CreateFolderPath 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5a10aa5e-3f25-4ec3-a0b9-284c30918a1f
description: 操作 CreateFolderPath EWS についての情報を検索します。
ms.openlocfilehash: 22561e5086c144e25d7e04b68ec6674b87c4718d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759819"
---
# <a name="createfolderpath-operation"></a>CreateFolderPath 操作

**CreateFolderPath** EWS の操作に関する情報を検索します。 
  
**CreateFolderPath**操作は、フォルダー階層を作成します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-createfolderpath-operation"></a>CreateFolderPath 操作を使用します。

**CreateFolderPath**操作の要求は、フォルダーおよび親フォルダーの識別子の配列を受け取るし、配列内のフォルダーの順序に基づいて、フォルダー階層を作成します。 
  
### <a name="createfolderpath-operation-soap-headers"></a>CreateFolderPath 操作の SOAP ヘッダー

**CreateFolderPath**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |**日付**プロパティのタイム ゾーンの範囲を識別します。 このヘッダーは、要求に適用されます。  <br/> |
   
## <a name="createfolderpath-operation-request-example-create-a-folder-hierarchy"></a>CreateFolderPath 操作の要求の例: フォルダーの階層を作成します。

**CreateFolderPath**操作要求の次の使用例は、3 つのフォルダーは、フォルダー階層を作成する方法を示しています。 既定の受信トレイ フォルダーの深さです。 
  
> [!NOTE]
> すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:CreateFolderPath>
         <m:ParentFolderId>
            <t:DistinguishedFolderId Id="inbox"/>
         </m:ParentFolderId>
         <m:RelativeFolderPath>
            <t:Folder>
               <t:DisplayName>MyFirstLevelFolder</t:DisplayName>
            </t:Folder>
            <t:Folder>
               <t:DisplayName>MySecondLevelFolder</t:DisplayName>
            </t:Folder>
            <t:Folder>
               <t:DisplayName>MyThirdLevelFolder</t:DisplayName>
            </t:Folder>
         </m:RelativeFolderPath>
      </m:CreateFolderPath>
   </soap:Body>
</soap:Envelope>

```

要求 SOAP 本体にはには、次の要素が含まれています。
  
- [CreateFolderPath](createfolderpath.md)
    
- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [RelativeFolderPath](relativefolderpath.md)
    
- [Folder](folder.md)
    
- [表示名 (文字列)](displayname-string.md)
    
## <a name="successful-createfolderpath-operation-response"></a>CreateFolderPath 操作の成功の応答

次の使用例は、正常な 3 つの階層のフォルダーにフォルダーを作成する**CreateFolderPath**操作の要求に応答を示しています。 既定の受信トレイ フォルダーの深さです。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:CreateFolderPathResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTExYisXAAA=" ChangeKey="AQAAABYAABq6Wxb"/>
                     <t:DisplayName>MyFirstLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTExm4QrAABqxisYAAA=" ChangeKey="AQAAABYAAAm4QrAABq6Wxg"/>
                     <t:DisplayName>MySecondLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTAABqxisZAAA=" ChangeKey="AQAAABYAA6Wxl"/>
                     <t:DisplayName>MyThirdLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
         </m:ResponseMessages>
      </m:CreateFolderPathResponse>
   </s:Body>
</s:Envelope>

```

応答 SOAP 本文には、次の要素が含まれています。
  
- [CreateFolderPathResponse](createfolderpathresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateFolderPathResponseMessage](createfolderpathresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [フォルダー Id](folderid.md)
    
- [表示名 (文字列)](displayname-string.md)
    
- [TotalCount](totalcount.md)
    
- [ChildFolderCount](childfoldercount.md)
    
- [UnreadCount](unreadcount.md)
    
## <a name="createfolderpath-operation-error-response"></a>CreateFolderPath 操作のエラー応答

**CreateFolderPath**操作の要求に対してエラー応答の例を次に示します。 これは、最初のうちに設定された表示名のプロパティの種類がない 2 つのフォルダーを作成する要求に応答します。 せず、表示名のプロパティでは、階層内の最初のフォルダーを作成することはできませんし、階層内の親フォルダーが作成されなかったために、2 番目のフォルダーを作成できません。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:CreateFolderPathResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:CreateFolderPathResponseMessage ResponseClass="Error">
               <m:MessageText>The folder save operation failed due to invalid property values.</m:MessageText>
               <m:ResponseCode>ErrorFolderSavePropertyError</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:MessageXml>
                  <t:FieldURI FieldURI="folder:DisplayName"/>
               </m:MessageXml>
               <m:Folders/>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Error">
               <m:MessageText>The specified parent folder could not be found.</m:MessageText>
               <m:ResponseCode>ErrorParentFolderNotFound</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:Folders/>
            </m:CreateFolderPathResponseMessage>
         </m:ResponseMessages>
      </m:CreateFolderPathResponse>
   </s:Body>
</s:Envelope>

```

エラー応答 SOAP 本体にはには、次の要素が含まれています。
  
- [CreateFolderPathResponse](createfolderpathresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateFolderPathResponseMessage](createfolderpathresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [MessageXml](messagexml.md)
    
- [FieldURI](fielduri.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。
  
## <a name="see-also"></a>関連項目

- [Exchange での EWS の操作](ews-operations-in-exchange.md)
    
- 
  [FindFolder 操作](findfolder-operation.md)
    

