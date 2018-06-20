---
title: InternalReply
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalReply
api_type:
- schema
ms.assetid: 1d784ded-b874-4eb1-8f6d-2e0e03330e1e
description: InternalReply 要素には、外出中 (OOF) 応答を送信するユーザーのドメインまたは信頼されるドメイン内の他のユーザーの出力が含まれています。
ms.openlocfilehash: ac5e9eadac7f45c233007ffb05f4d2430875ec52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831955"
---
# <a name="internalreply"></a>InternalReply

**InternalReply**要素には、外出中 (OOF) 応答を送信するユーザーのドメインまたは信頼されるドメイン内の他のユーザーの出力が含まれています。 
  
```XML
<InternalReply>
   <Message/> 
</InternalReply>
```

 **ReplyBody**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|xml:lang  <br/> |**InternalReply**メッセージで使用される言語を指定します。 この属性に指定できる値は、IETF RFC 3066 で定義されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[メッセージ (可用性)](message-availability.md) <br/> |不在時の応答が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |不在の設定を指定します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |不在の設定が含まれています。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

SetUserOofSettings 要求の次の使用例は、 [OofState](oofstate.md)を**有効**に設定、10 日間、不在時の期間を設定し、内部と外部の OOF メッセージを設定します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserOofSettings 操作](getuseroofsettings-operation.md)
  
[SetUserOofSettings 操作](setuseroofsettings-operation.md)

