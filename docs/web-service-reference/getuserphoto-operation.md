---
title: GetUserPhoto 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: 操作 GetUserPhoto EWS についての情報を検索します。
ms.openlocfilehash: 4465ac7115d96f5b6ef39e467663c9bf1c70e99e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831694"
---
# <a name="getuserphoto-operation"></a>GetUserPhoto 操作

**GetUserPhoto** EWS の操作に関する情報を検索します。 
  
**GetUserPhoto**操作は、Active Directory ドメイン サービス (AD DS) からのユーザーの写真を取得します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getuserphoto-operation"></a>GetUserPhoto 操作を使用します。

**RemoveContactFromImList**操作は、単純な操作をユーザーの電子メール アドレスと要求された写真のサイズを受け取り、応答でフォト ストリームを返します。 
  
> [!NOTE]
> EWS が、SOAP と REST ベースの操作の両方がユーザーの写真を取得します。 REST インターフェイスの詳細については、 [Exchange での EWS を使用して、ユーザーの写真の取り込み](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)を参照してください。 
  
### <a name="getuserphoto-operation-soap-headers"></a>GetUserPhoto 操作の SOAP ヘッダー

**GetUserPhoto**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a>GetUserPhoto 操作の要求の使用例: ユーザーの写真を取得します。

**GetUserPhoto**操作要求の次の例では、ユーザーの写真を取得する方法を示します。 次の使用例は、48 x 48 ピクセル、ユーザーの写真を要求します。 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>user1@contoso.com</m:Email>
         <m:SizeRequested>HR48x48</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>
```

次の要素は、SOAP 本文の要求で使用されます。
  
- [GetUserPhoto](getuserphoto.md)
    
- [電子メール (文字列)](email-string.md)
    
- [SizeRequested](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a>GetUserPhoto 操作の成功の応答

次の例では、ユーザーの写真を取得するのには、 **GetUserPhoto**の操作を正常な応答を示します。 
  
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
      <GetUserPhotoResponse ResponseClass="Success" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <HasChanged>true</HasChanged>
         <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/02</PictureData>
      </GetUserPhotoResponse>
   </s:Body>
</s:Envelope>

```

応答 SOAP 本文では、次の要素が使用されます。
  
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [HasChanged](haschanged.md)
    
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a>GetUserPhoto 操作のエラー応答

組織に存在しない電子メール アドレスのユーザーの写真を取得しようとした場合に、SOAP エンベロープはエラー コードを返しません。 500 HTTP ステータス コードは、要求が失敗したことを示す応答で返されます。 
  
## <a name="see-also"></a>関連項目

- [Exchange での EWS の操作](ews-operations-in-exchange.md)   
- [EWS を使用して Exchange でのユーザーの写真を取り込み](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

