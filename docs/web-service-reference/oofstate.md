---
title: OofState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofState
api_type:
- schema
ms.assetid: 3c486a38-06da-4382-ad20-664d067d76ac
description: 取得またはユーザーの Office (OOF) の状態を設定する OofState 要素を使用します。
ms.openlocfilehash: f97c050aec102b384fa4d98e6dee43befd4dc9ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832651"
---
# <a name="oofstate"></a>OofState

取得またはユーザーの Office (OOF) の状態を設定する**OofState**要素を使用します。 
  
```xml
<OofState>Disabled or Enabled or Scheduled</OofState>
```

 **OofState**
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

テキスト値は、 **OofState**要素の必要があります。 次の一覧には、この要素の有効な値が含まれています。 
  
- **無効になっています。**
    
- **Enabled**
    
- **スケジュール**
    
**[スケジュール済]** の値は、[期間 (UserOofSettings)](duration-useroofsettings.md)の要素で指定された期間内に、不在の状態が**有効**に設定されていることを示します。 
  
## <a name="remarks"></a>備考

SetUsersOofSettingRequest メッセージと、GetUserOofSettingResponse メッセージの両方では、この要素が必要です。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="example"></a>例

SetUserOofSettings 要求の次の使用例は、 **OofState**を有効にします。
  
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

