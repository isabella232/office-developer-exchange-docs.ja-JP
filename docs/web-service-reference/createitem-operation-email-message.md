---
title: CreateItem 操作 (メール メッセージ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1
description: CreateItem 操作は、電子メール メッセージの作成に使用されます。
ms.openlocfilehash: 74784d72ed14fa139c616cd11740a62efd17b338
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536469"
---
# <a name="createitem-operation-email-message"></a>CreateItem 操作 (メール メッセージ)

CreateItem 操作は、電子メール メッセージの作成に使用されます。
  
## <a name="createitem-request-example"></a>CreateItem 要求の例

### <a name="description"></a>説明

CreateItem 要求の次の例は、新しい電子メール メッセージを作成し、メッセージを送信し、そのコピーを下書きフォルダーに保存する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem MessageDisposition="SendAndSaveCopy" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </SavedItemFolderId>
      <Items>
        <t:Message>
          <t:ItemClass>IPM.Note</t:ItemClass>
          <t:Subject>Project Action</t:Subject>
          <t:Body BodyType="Text">Priority - Update specification</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sschmidt@example.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
          <t:IsRead>false</t:IsRead>
        </t:Message>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。 
  
- [CreateItem](createitem.md)
    
- [SavedItemFolderId](saveditemfolderid.md)
    
- [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [ItemClass](itemclass.md)
    
- [件名](subject.md)
    
- [Body](body.md)
    
- [ToRecipients](torecipients.md)
    
- [メールボックス](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [IsRead](isread.md)
    
CreateItem 操作の要求メッセージの他のオプションを見つけるには、スキーマ階層を確認します。 [CreateItem 要素から開始](createitem.md)します。 
  
## <a name="successful-createitem-response"></a>CreateItem 応答の成功

### <a name="description"></a>説明

次の例は、CreateItem 要求に対する正常な応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>成功した応答要素

応答には、次の要素が含まれます。 
  
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
CreateItem 操作の応答メッセージの他のオプションを見つけるには、スキーマ階層を確認します。 [CreateItemResponse 要素から開始](createitemresponse.md)します。 
  
## <a name="error-createitem-response"></a>エラー CreateItem 応答

### <a name="description"></a>説明

次の例は、CreateItem 要求に対するエラー応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>The user account which was used to submit this request does not have the right to send mail on behalf of the specified sending account.</m:MessageText>
          <m:ResponseCode>ErrorSendAsDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>エラー応答要素

エラー応答では、次の要素が使用されます。 
  
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Items](items.md)
    
CreateItem 操作のエラー応答メッセージの他のオプションを見つけるには、スキーマ階層を確認します。 [CreateItemResponse 要素から開始](createitemresponse.md)します。 
  
## <a name="see-also"></a>関連項目



[CreateItem 操作](createitem-operation.md)

