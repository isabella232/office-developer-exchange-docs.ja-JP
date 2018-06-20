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
description: ExternalAudience 要素を設定または外部の Office (OOF) メッセージを送信するかを決定する値が含まれています。
ms.openlocfilehash: 836b0f6a5140a37e1584f571cb8e26534fe7a25f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760426"
---
# <a name="externalaudience"></a>ExternalAudience

**ExternalAudience**要素を設定または外部の Office (OOF) メッセージを送信するかを決定する値が含まれています。 
  
```xml
<ExternalAudience>None or Known or All</ExternalAudience>
```

 **ExternalAudience**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |不在の設定を指定します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |不在の設定が含まれています。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、この要素の必要があります。 次の表は、この要素の有効な値を一覧します。
  
|**値**|**説明**|
|:-----|:-----|
|**None** <br/> |メールボックス ユーザーの組織外のユーザーにメッセージを送信するメールの送信者は、外部の OOF メッセージの応答を受信しません。  <br/> |
|**呼ばれる** <br/> |メールボックス ユーザーの組織の外部ユーザーへのメッセージのみが表示されます、外部の OOF メッセージ応答送信者がユーザーの Exchange の場合に送信したメールの送信者は、連絡先リストを保存します。  <br/> |
|**All** <br/> |メールボックス ユーザーの組織外のユーザーにメッセージを送信するメールの送信者が外部の OOF メッセージの応答を受け取ります。  <br/> |
   
## <a name="remarks"></a>備考

この要素は、 [AllowExternalOof](allowexternaloof.md)要素と同じ型を共有します。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="example"></a>例

SetUserOofSettings 要求の次の使用例、OoFState を**有効**に設定に**すべて**の外部の対象ユーザーの設定、不在時の期間を 10 日に設定、内部と外部の OOF メッセージを設定します。
  
```
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

