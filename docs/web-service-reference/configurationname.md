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
description: ConfigurationName 要素は、名前によって要求されたサービスの構成を指定します。
ms.openlocfilehash: a03a0bc0ab7ecbc1c2aec31f864503ee0f560908
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759651"
---
# <a name="configurationname"></a>ConfigurationName

**ConfigurationName**要素は、名前によって要求されたサービスの構成を指定します。 
  
```xml
<ConfigurationName>MailTips or UnifiedMessagingConfiguration or ProtectionRules</ConfigurationName>
```

 **ServiceConfigurationType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RequestedConfiguration](requestedconfiguration.md) <br/> |要求されたサービスの構成が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

**ConfigurationName**要素の有効な値を次の表に一覧します。 
  
**ConfigurationName 要素の値**

|**値**|**説明**|
|:-----|:-----|
|メール ヒント  <br/> |メール ヒント サービスの構成を識別します。  <br/> |
|UnifiedMessagingConfiguration  <br/> |ユニファイド メッセージング サービスの構成を識別します。  <br/> |
|ProtectionRules  <br/> |保護ルールのサービスの構成を識別します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

