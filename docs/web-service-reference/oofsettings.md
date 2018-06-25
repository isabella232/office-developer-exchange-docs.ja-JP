---
title: OofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofSettings
api_type:
- schema
ms.assetid: 8f37d174-db11-427c-bbed-fdde754a60c7
description: OofSettings 要素には、Office (OOF) の設定が含まれています。
ms.openlocfilehash: d71f068ff24af22da98b6b4de090ab26d3f74f26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832649"
---
# <a name="oofsettings"></a>OofSettings

**OofSettings**要素には、Office (OOF) の設定が含まれています。 
  
[GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
  
[OofSettings](oofsettings.md)
  
```xml
<OofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</OofSettings>
```

 **UserOofSettings**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[OofState](oofstate.md) <br/> |ユーザーの不在時の状態が含まれています。  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |外部の OOF メッセージを送信するかを決定する値が含まれています。  <br/> |
|[期間 (UserOofSettings)](duration-useroofsettings.md) <br/> |不在の状態が有効である[OofState](oofstate.md)要素は、**スケジュール**に設定されている場合の期間が含まれています。 [OofState](oofstate.md)要素は、**有効**または**無効**に設定されている場合、この要素の値は無視されます。  <br/> |
|[InternalReply](internalreply.md) <br/> |ユーザーのドメインまたは信頼されたドメイン内の他のユーザーに送信される不在時の応答が含まれています。  <br/> |
|[ExternalReply](externalreply.md) <br/> |受信者のドメインまたは信頼されるドメインの外部アドレスに送信される不在時の応答が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |応答結果とユーザーの不在時の設定が含まれています。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserOofSettings 操作](getuseroofsettings-operation.md)
  
[SetUserOofSettings 操作](setuseroofsettings-operation.md)

