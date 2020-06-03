---
title: ExternalAudience
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExternalAudience
api_type:
- schema
ms.assetid: 79dc2a4c-f7dd-46d1-8f31-149116e1f76e
description: ExternalAudience 要素は、外部不在 (OOF) メッセージが送信されるユーザーを決定する値を設定または格納します。
ms.openlocfilehash: b3fcebd9042b07bb9a8294196799ef2a13d78bdd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530601"
---
# <a name="externalaudience"></a>ExternalAudience

**Externalaudience**要素は、外部不在 (OOF) メッセージが送信されるユーザーを決定する値を設定または格納します。 
  
```xml
<ExternalAudience>None or Known or All</ExternalAudience>
```

 **ExternalAudience**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |OOF 設定を指定します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |不在時の設定が含まれます。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a>テキスト値

この要素にはテキスト値が必要です。 次の表に、この要素で使用できる値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|**なし** <br/> |メールボックスユーザーの組織外の電子メール送信者は、ユーザーにメッセージを送信すると、外部の不在時メッセージ応答を受信しません。  <br/> |
|**一般的** <br/> |メールボックスユーザーの組織外の電子メール送信者がユーザーにメッセージを送信すると、送信者がユーザーの Exchange ストアの連絡先リストにある場合にのみ、外部の OOF メッセージ応答が受信されます。  <br/> |
|**All** <br/> |メールボックスユーザーの組織外の電子メール送信者は、ユーザーにメッセージを送信すると、外部の OOF メッセージ応答を受信します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は、 [AllowExternalOof](allowexternaloof.md)要素と同じ型を共有します。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

SetUserOofSettings 要求の次の例では、OoFState を**Enabled**に設定し、外部対象ユーザーを**すべて**に設定し、oof の時間を10日に設定し、内部および外部の oof メッセージを設定します。
  
```
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
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserOofSettings 操作](getuseroofsettings-operation.md)
  
[SetUserOofSettings 操作](setuseroofsettings-operation.md)

