---
title: Mailbox (Availability)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Mailbox
api_type:
- schema
ms.assetid: affd192e-8914-473f-9098-d9bdf898de2c
description: Mailbox 要素は、SetUserOofSettings または GetUserOofSettings 要求のメールボックス ユーザーを表します。
ms.openlocfilehash: 5e32c4be807dae92b27df7012caa8eb1b295b26c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522923"
---
# <a name="mailbox-availability"></a>Mailbox (Availability)

**Mailbox 要素** は、SetUserOofSettings または GetUserOofSettings 要求のメールボックス ユーザーを表します。 
  
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
|[Name (EmailAddress)](name-emailaddress.md) <br/> |メールボックス ユーザーの表示名を表します。 この要素は、SetUserOofSettingsRequest のオプションです。 GetUserOofSettingsRequest は、この要素を返します。  <br/> |
|[Address (string)](address-string.md) <br/> |メールボックス ユーザーの電子メール アドレスを表します。 この要素は必須です。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |メッセージのルーティング プロトコルを表します。 この要素は、SetUserOofSettingsRequest のオプションです。 GetUserOofSettingsRequest は、この要素を返します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserOofSettingsRequest](getuseroofsettingsrequest.md) <br/> |メールボックス ユーザーの [無効] (OOF) Officeメッセージを取得するために使用します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |メールボックス ユーザーの OOF 設定とメッセージを設定するために使用します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>注釈

電子メール アドレスは、OOF 設定を含む予定表フォルダーを識別するために使用されます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserOofSettings 操作](getuseroofsettings-operation.md)
- [SetUserOofSettings 操作](setuseroofsettings-operation.md)

