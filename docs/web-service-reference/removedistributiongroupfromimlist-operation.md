---
title: RemoveDistributionGroupFromImList 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 252bddf2-98b6-4824-b548-2fba2bda5384
description: 操作 RemoveDistributionGroupFromImList EWS についての情報を検索します。
ms.openlocfilehash: 9999f98a5698dd33c22e22fdf86bd00a2d053b52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833096"
---
# <a name="removedistributiongroupfromimlist-operation"></a>RemoveDistributionGroupFromImList 操作

**RemoveDistributionGroupFromImList** EWS の操作に関する情報を検索します。 
  
**RemoveDistributionGroupFromImList**操作は、Lync は、連絡先ストアの Exchange を使用すると、Lync のインスタント メッセージング (IM) の一覧から配布グループを削除します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-removedistributiongroupfromimlist-operation"></a>RemoveDistributionGroupFromImList 操作を使用します。

**RemoveDistributionGroupFromImList**操作は、Exchange サーバーに格納されている Lync の IM のリストから削除する配布グループを識別する 1 つの引数を受け取ります。 
  
### <a name="removedistributiongroupfromimlist-operation-soap-headers"></a>RemoveDistributionGroupFromImList 操作の SOAP ヘッダー

**RemoveDistributionGroupFromImList**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="removedistributiongroupfromimlist-operation-request-example-remove-a-distribution-group-from-an-im-list"></a>RemoveDistributionGroupFromImList 操作の要求の例: 配布グループの IM のリストから削除

**RemoveDistributionGroupFromImList**操作要求の次の例では、IM グループから配布グループを削除する方法を示します。 **RemoveDistributionGroupFromImList**操作では、IM のリストから削除する配布グループを識別する一意のグループ id を受け入れます。 [GetImItemList 操作](getimitemlist-operation.md)および[AddDistributionGroupToImList 操作](adddistributiongrouptoimlist-operation.md)の応答で返される[ExchangeStoreId](exchangestoreid.md)要素は、IM のリストから削除することができる配布グループを識別します。 
  
> [!NOTE]
> すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。 
  
```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:RemoveDistributionGroupFromImList>
         <m:GroupId Id="AAMkADEzO4QrAABmEh5oAAA="/>
      </m:RemoveDistributionGroupFromImList>
   </soap:Body>
</soap:Envelope>
```

次の要素は、SOAP 本文の要求で使用されます。
  
- [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md)
    
- [グループ Id](groupid.md)
    
## <a name="successful-removedistributiongroupfromimlist-operation-response"></a>RemoveDistributionGroupFromImList 操作の成功の応答

次の例では、IM グループから配布グループの削除] に成功した要求への応答、 **RemoveDistributionGroupFromImList**の操作を示します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveDistributionGroupFromImListResponse ResponseClass="Success" 
                                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

応答 SOAP 本文では、次の要素が使用されます。
  
- [RemoveDistributionGroupFromImListResponse](removedistributiongroupfromimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removedistributiongroupfromimlist-operation-error-response-example"></a>RemoveDistributionGroupFromImList 操作のエラー応答の例

**RemoveDistributionGroupFromImList**操作の要求に対してエラー応答の例を次に示します。 これは、メールボックスから既に削除されている配布グループを削除する要求に応答します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveDistributionGroupFromImListResponse ResponseClass="Error" 
                                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本文では、次の要素が使用されます。
  
- [RemoveDistributionGroupFromImListResponse](removedistributiongroupfromimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>関連項目

- [Exchange での EWS の操作](ews-operations-in-exchange.md)
    
- [GetImItemList 操作](getimitemlist-operation.md)
    
- [AddDistributionGroupToImList 操作](adddistributiongrouptoimlist-operation.md)
    
- [Exchange 内の EWS のユーザーと連絡先](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx#What)
    

