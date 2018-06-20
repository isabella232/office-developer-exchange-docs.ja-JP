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
description: メールボックス要素では、メールボックス ユーザーを表すを SetUserOofSettings のか、GetUserOofSettings を要求します。
ms.openlocfilehash: 2e901ae0df56542f56f247184254294735018468
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832254"
---
# <a name="mailbox-availability"></a>メールボックス (可用性)

**メールボックス**要素では、メールボックス ユーザーを表すを SetUserOofSettings のか、GetUserOofSettings を要求します。 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[名 (EmailAddress)](name-emailaddress.md) <br/> |メールボックス ユーザーの表示名を表します。 この要素では、SetUserOofSettingsRequest では省略可能です。 GetUserOofSettingsRequest には、この要素が返されます。  <br/> |
|[アドレス (文字列)](address-string.md) <br/> |メールボックス ユーザーの電子メール アドレスを表します。 この要素は必須です。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |メッセージのルーティング プロトコルを表します。 この要素では、SetUserOofSettingsRequest では省略可能です。 GetUserOofSettingsRequest には、この要素が返されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserOofSettingsRequest](getuseroofsettingsrequest.md) <br/> |メールボックス ユーザーの Office (OOF) の設定とメッセージの取得に使用されます。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |メールボックス ユーザーの不在時の設定とメッセージの設定に使用されます。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>備考

電子メール アドレスを使用して、不在時の設定が含まれている予定表フォルダーを識別します。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserOofSettings 操作](getuseroofsettings-operation.md)
- [SetUserOofSettings 操作](setuseroofsettings-operation.md)

