---
title: ConfigurationName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConfigurationName
api_type:
- schema
ms.assetid: 3b524a2f-9c6b-4550-9f3d-f78d176b0f7b
description: ConfigurationName 要素は、要求されたサービス構成を名前で指定します。
ms.openlocfilehash: 39f847c256614cd0c207f440691bd87d09ed237b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523126"
---
# <a name="configurationname"></a>ConfigurationName

**ConfigurationName 要素は**、要求されたサービス構成を名前で指定します。 
  
```xml
<ConfigurationName>MailTips or UnifiedMessagingConfiguration or ProtectionRules</ConfigurationName>
```

 **ServiceConfigurationType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RequestedConfiguration](requestedconfiguration.md) <br/> |要求されたサービス構成が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、ConfigurationName** 要素に使用できる値を示します。 
  
**ConfigurationName 要素の値**

|**値**|**説明**|
|:-----|:-----|
|メール ヒント  <br/> |MailTips サービス構成を識別します。  <br/> |
|UnifiedMessagingConfiguration  <br/> |ユニファイド メッセージング サービスの構成を識別します。  <br/> |
|ProtectionRules  <br/> |Protection Rules サービス構成を識別します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

