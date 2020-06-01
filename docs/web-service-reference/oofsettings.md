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
description: OofSettings 要素には、不在 (OOF) の設定が含まれています。
ms.openlocfilehash: c1b214fd8bfab5b7a82d41a5187cf6e0fc4ba79c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467194"
---
# <a name="oofsettings"></a>OofSettings

**Oofsettings**要素には、不在 (OOF) の設定が含まれています。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[OofState](oofstate.md) <br/> |ユーザーの不在時の状態を格納します。  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |外部の OOF メッセージが送信されるユーザーを決定する値を格納します。  <br/> |
|[Duration (UserOofSettings)](duration-useroofsettings.md) <br/> |[Oofstate](oofstate.md)要素が [**スケジュール済み**] に設定されている場合に、OOF の状態が有効になる期間を含みます。 [Oofstate](oofstate.md)要素が**Enabled**または**Disabled**に設定されている場合、この要素の値は無視されます。  <br/> |
|[InternalReply](internalreply.md) <br/> |ユーザーのドメインまたは信頼されたドメイン内の他のユーザーに送信される OOF 応答を含みます。  <br/> |
|[ExternalReply](externalreply.md) <br/> |受信者のドメインまたは信頼されたドメイン外のアドレスに送信される OOF 応答を含みます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |応答結果とユーザーの OOF 設定が含まれます。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserOofSettings 操作](getuseroofsettings-operation.md)
  
[SetUserOofSettings 操作](setuseroofsettings-operation.md)

