---
title: InternalReply
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InternalReply
api_type:
- schema
ms.assetid: 1d784ded-b874-4eb1-8f6d-2e0e03330e1e
description: InternalReply 要素には、ユーザーのドメインまたは信頼できるドメイン内の他のユーザーに送信される、アウトオブオフィス (OOF) 応答が含まれる。
ms.openlocfilehash: bbf25d05330463e44d9c865749943ed45a64e157
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541106"
---
# <a name="internalreply"></a>InternalReply

**InternalReply 要素** には、ユーザーのドメインまたは信頼できるドメイン内の他のユーザーに送信される、アウトオブオフィス (OOF) 応答が含まれる。 
  
```XML
<InternalReply>
   <Message/> 
</InternalReply>
```

 **ReplyBody**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|xml:lang  <br/> |InternalReply メッセージで使用 **される言語を指定** します。 この属性の可能な値は、IETF RFC 3066 によって定義されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Message (Availability)](message-availability.md) <br/> |OOF 応答が含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |OOF 設定を指定します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |OOF 設定が含まれる。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

SetUserOofSettings 要求の次の例では [、OofState](oofstate.md) を **Enabled** に設定し、OOF の期間を 10 日間設定し、内部および外部の OOF メッセージを設定します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserOofSettings 操作](getuseroofsettings-operation.md)
  
[SetUserOofSettings 操作](setuseroofsettings-operation.md)

