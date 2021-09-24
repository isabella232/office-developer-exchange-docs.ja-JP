---
title: OofState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OofState
api_type:
- schema
ms.assetid: 3c486a38-06da-4382-ad20-664d067d76ac
description: OofState 要素を使用して、ユーザーのアウト オブ Office (OOF) 状態を取得または設定します。
ms.openlocfilehash: 4d0d893e364fc85d36e37400538a336473832efd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509538"
---
# <a name="oofstate"></a>OofState

**OofState** 要素は、ユーザーの Out of the Office (OOF) 状態を取得または設定するために使用されます。 
  
```xml
<OofState>Disabled or Enabled or Scheduled</OofState>
```

 **OofState**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |OOF 設定を指定します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |OOF 設定が含まれる。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a>テキスト値

OofState 要素にはテキスト **値が必要** です。 次の一覧には、この要素に使用できる値が含まれます。 
  
- **Disabled**
    
- **Enabled (有効)**
    
- **スケジュール済み**
    
値 Scheduled は **、期間** [(UserOofSettings)](duration-useroofsettings.md)要素によって識別される期間中に OOF の状態が [有効] に設定されています。  
  
## <a name="remarks"></a>注釈

この要素は、SetUsersOofSettingRequest メッセージと GetUserOofSettingResponse メッセージの両方で必要です。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

SetUserOofSettings 要求の次の例では **、OofState を有効にしています**。
  
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
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserOofSettings 操作](getuseroofsettings-operation.md)
  
[SetUserOofSettings 操作](setuseroofsettings-operation.md)

