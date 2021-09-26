---
title: OofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OofSettings
api_type:
- schema
ms.assetid: 8f37d174-db11-427c-bbed-fdde754a60c7
description: OofSettings 要素には、オブジェクト外 (OOF) Office設定が含まれる。
ms.openlocfilehash: 0a612cacb69464dfda3c1f235c32f569d3e45775
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543171"
---
# <a name="oofsettings"></a>OofSettings

**OofSettings 要素には**、オブジェクト外 (OOF) Office設定が含まれる。 
  
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
|[OofState](oofstate.md) <br/> |ユーザーの OOF 状態を格納します。  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |外部 OOF メッセージの送信先を決定する値が含まれます。  <br/> |
|[Duration (UserOofSettings)](duration-useroofsettings.md) <br/> |[OofState](oofstate.md)要素が [スケジュール済み] に設定されている場合に OOF 状態が有効になっている期間を格納 **します**。 [OofState 要素が](oofstate.md)Enabled または **Disabled** に設定 **されている** 場合、この要素の値は無視されます。  <br/> |
|[InternalReply](internalreply.md) <br/> |ユーザーのドメインまたは信頼されたドメイン内の他のユーザーに送信される OOF 応答が含まれる。  <br/> |
|[ExternalReply](externalreply.md) <br/> |受信者のドメインまたは信頼できるドメイン外のアドレスに送信される OOF 応答が含まれます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |応答結果とユーザーの OOF 設定が含まれる。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserOofSettings 操作](getuseroofsettings-operation.md)
  
[SetUserOofSettings 操作](setuseroofsettings-operation.md)

