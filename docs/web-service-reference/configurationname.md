---
title: ConfigurationName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConfigurationName
api_type:
- schema
ms.assetid: 3b524a2f-9c6b-4550-9f3d-f78d176b0f7b
description: ConfigurationName 要素は、要求されたサービス構成を名前で指定します。
ms.openlocfilehash: 5e1216253a633af643dbd276827842dbe2db5d5f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463924"
---
# <a name="configurationname"></a>ConfigurationName

**ConfigurationName**要素は、要求されたサービス構成を名前で指定します。 
  
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
|[RequestedConfiguration](requestedconfiguration.md) <br/> |要求されたサービス構成を含みます。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、 **ConfigurationName**要素に指定できる値を示します。 
  
**ConfigurationName 要素の値**

|**値**|**説明**|
|:-----|:-----|
|メール ヒント  <br/> |メールヒントサービスの構成を識別します。  <br/> |
|UnifiedMessagingConfiguration  <br/> |ユニファイドメッセージングサービスの構成を識別します。  <br/> |
|ProtectionRules  <br/> |保護ルールサービスの構成を識別します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

