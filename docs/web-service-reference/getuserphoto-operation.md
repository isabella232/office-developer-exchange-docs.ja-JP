---
title: GetUserPhoto 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: GetUserPhoto EWS 操作に関する情報を検索します。
ms.openlocfilehash: 6dd1ce73d6291e60ce188b98b917a4c79ce792b5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547485"
---
# <a name="getuserphoto-operation"></a>GetUserPhoto 操作

**GetUserPhoto** EWS 操作に関する情報を検索します。 
  
**GetUserPhoto 操作は**、Active Directory ドメイン サービス (DS) からユーザー ADします。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getuserphoto-operation"></a>GetUserPhoto 操作の使用

**RemoveContactFromImList** 操作は、ユーザーの電子メール アドレスと要求された写真サイズを受け入れ、応答で写真ストリームを返す簡単な操作です。 
  
> [!NOTE]
> EWS には、ユーザーの写真を取得する SOAP と REST ベースの操作の両方があります。 REST インターフェイスの詳細については、「EWS を使用してユーザーの写真を取得する」[を参照Exchange。](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx) 
  
### <a name="getuserphoto-operation-soap-headers"></a>GetUserPhoto 操作 SOAP ヘッダー

**GetUserPhoto 操作では**、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**Element**|**説明**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a>GetUserPhoto 操作要求の例: ユーザーの写真を取得する

**GetUserPhoto 操作要求の次の例** は、ユーザーの写真を取得する方法を示しています。 次の使用例は、48x48 ピクセルのユーザー写真を要求します。 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

要求 SOAP 本文では、次の要素が使用されます。
  
- [GetUserPhoto](getuserphoto.md)
    
- [Email (String)](email-string.md)
    
- [SizeRequested](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a>GetUserPhoto 操作の正常な応答

次の例は、ユーザーの写真を取得する **GetUserPhoto** 操作に対する正常な応答を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserPhotoResponse ResponseClass="Success" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
    
## <a name="getuserphoto-operation-error-response"></a>GetUserPhoto 操作エラー応答

組織内に存在しない電子メール アドレスのユーザー写真を取得しようとした場合、SOAP エンベロープはエラー コードを返しません。 要求が失敗したと示す 500 HTTP 状態コードが応答で返されます。 
  
## <a name="see-also"></a>関連項目

- [EWS 操作 (Exchange](ews-operations-in-exchange.md)   
- [Exchange で EWS を使用してユーザーの写真を取得する](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

