---
title: メールボックス (可用性)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: affd192e-8914-473f-9098-d9bdf898de2c
description: Mailbox 要素は、SetUserOofSettings または GetUserOofSettings 要求のメールボックスユーザーを表します。
ms.openlocfilehash: 1bda6e8b90551b86b4e1c2711ac25693a65e5410
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458076"
---
# <a name="mailbox-availability"></a>メールボックス (可用性)

**Mailbox**要素は、SetUserOofSettings または getuseroofsettings 要求のメールボックスユーザーを表します。 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Name (EmailAddress)](name-emailaddress.md) <br/> |メールボックスユーザーの表示名を表します。 この要素は、SetUserOofSettingsRequest では省略可能です。 GetUserOofSettingsRequest は、この要素を返します。  <br/> |
|[Address (string)](address-string.md) <br/> |メールボックスユーザーの電子メールアドレスを表します。 この要素は必須です。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |メッセージのルーティングプロトコルを表します。 この要素は、SetUserOofSettingsRequest では省略可能です。 GetUserOofSettingsRequest は、この要素を返します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserOofSettingsRequest](getuseroofsettingsrequest.md) <br/> |メールボックスユーザーの不在時 (OOF) の設定とメッセージを取得するために使用されます。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |メールボックスユーザーの不在時の設定とメッセージを設定するために使用します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>注釈

この電子メールアドレスは、OOF 設定を含む予定表フォルダーを識別するために使用されます。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserOofSettings 操作](getuseroofsettings-operation.md)
- [SetUserOofSettings 操作](setuseroofsettings-operation.md)

