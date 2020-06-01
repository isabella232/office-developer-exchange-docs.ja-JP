---
title: UpdateItem 操作 (連絡先)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 298fdd71-a83d-4407-9728-4f0a8e2d857c
description: UpdateItem 操作は、Exchange ストア内の連絡先アイテムのプロパティを更新するために使用されます。
ms.openlocfilehash: 66e1b91ea3154d8a501339aed7b398970e8f5392
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459827"
---
# <a name="updateitem-operation-contact"></a>UpdateItem 操作 (連絡先)

UpdateItem 操作は、Exchange ストア内の連絡先アイテムのプロパティを更新するために使用されます。
  
## <a name="updateitem-contact-request-example"></a>UpdateItem (Contact) 要求の例

### <a name="description"></a>説明

次のコード例は、連絡先の電子メールアドレスを更新する方法を示しています。
  
### <a name="code"></a>コード

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                ConflictResolution="AlwaysOverwrite">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAA=" ChangeKey="EQAAABYi" />
          <t:Updates>
            <t:SetItemField>
              <t:IndexedFieldURI FieldURI="contacts:EmailAddress" FieldIndex="EmailAddress1"/>
              <t:Contact>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">changedemail@example.com</t:Entry>
                </t:EmailAddresses>
              </t:Contact>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

アイテム識別子は読みやすくするために短縮されています。
  
### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Updates (Item)](updates-item.md)
    
- [SetItemField](setitemfield.md)
    
- [IndexedFieldURI](indexedfielduri.md)
    
- [連絡先](contact.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Entry (EmailAddress)](entry-emailaddress.md)
    
## <a name="successful-updateitem-contact-response"></a>成功した UpdateItem (連絡先) 応答

### <a name="description"></a>説明

次のコード例は、正常な UpdateItem 応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtAE=" ChangeKey="EQAAABYx" />
            </t:Contact>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

アイテム識別子は読みやすくするために短縮されています。
  
### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateItemResponse](updateitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateItemResponseMessage](updateitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [アイテム (非 Emptyarrayofallitemstype)](items-nonemptyarrayofallitemstype.md)
    
- [連絡先](contact.md)
    
- [ItemId](itemid.md)
    
## <a name="invalid-updateitem-contact-request-example"></a>無効な UpdateItem (連絡先) 要求の例

### <a name="description"></a>説明

次のコード例は、無効な要求を示しています。
  
### <a name="code"></a>コード

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                ConflictResolution="AlwaysOverwrite">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEF=" ChangeKey="EQAAABYi" />
          <t:Updates>
            <t:SetItemField>
              <t:IndexedFieldURI FieldURI="contacts:EmailAddress" FieldIndex="EmailAddress4"/>
              <t:Contact>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress4">changedemail2@example.com</t:Entry>
                </t:EmailAddresses>
              </t:Contact>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

アイテム識別子は読みやすくするために短縮されています。
  
## <a name="updateitem-contact-error-response"></a>UpdateItem (Contact) エラー応答

### <a name="description"></a>説明

次のコード例は、UpdateItem (連絡先) 要求に対するエラー応答を示しています。
  
### <a name="code"></a>コード

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <soap:faultcode>Client</soap:faultcode>
      <soap:faultstring>The request failed schema validation.</soap:faultstring>
      <detail>
        <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The 'Key' attribute is invalid - The value 'EmailAddress4' is invalid according to its data type 'https://schemas.microsoft.com/exchange/services/2006/types:EmailAddressKeyType' - The Enumeration constraint failed.</e:Message>
        <e:Line xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">17</e:Line>
        <e:Position xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">19</e:Position>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

スキーマ検証エラーによって発生したエラー応答の SOAP 本文で使用されている一部の要素は、メッセージまたは種類のスキーマで定義されていません。 **Detail**要素には、エラーに関する情報が含まれています。 応答[secの](responsecode.md)要素にエラーコードが含まれています。 [メッセージ](message-ex15websvcsotherref.md)要素には、エラーの説明が含まれています (使用可能な場合)。 **Line**要素は、スキーマ検証エラーが発生した行番号を示します。 **Position**要素は、XML ドキュメントの左端の文字からの位置を表します。 
  
## <a name="see-also"></a>関連項目




  [UpdateItem 操作](updateitem-operation.md)

