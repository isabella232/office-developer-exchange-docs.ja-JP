---
title: UnifiedMessagingConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UnifiedMessagingConfiguration
api_type:
- schema
ms.assetid: cbdb4268-077e-44ed-8ec2-9d759c84cc6d
description: UnifiedMessagingConfiguration 要素には、ユニファイド メッセージング サービスのサービス構成情報が含まれている。
ms.openlocfilehash: 861be041117a9df4329ed5b6995635aee3220003
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517498"
---
# <a name="unifiedmessagingconfiguration"></a>UnifiedMessagingConfiguration

**UnifiedMessagingConfiguration** 要素には、ユニファイド メッセージング サービスのサービス構成情報が含まれている。 
  
```XML
<UnifiedMessagingConfiguration>
   <UmEnabled/>
   <PlayOnPhoneDialString/>
   <PlayOnPhoneEnabled/>
</UnifiedMessagingConfiguration>
```

 **UnifiedMessageServiceConfiguration**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[UmEnabled](umenabled.md) <br/> |アカウントに対してユニファイド メッセージングが有効かどうかを示します。 この要素は必須です。  <br/> |
|[PlayOnPhoneDialString (Exchange Web サービス)](playonphonedialstring-exchange-web-services.md) <br/> |Play-on-電話を識別します。 この要素は必須です。  <br/> |
|[PlayOnPhoneEnabled](playonphoneenabled.md) <br/> |Play-on-電話機能が有効かどうかを示します。 この要素は必須です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |サービス構成設定が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
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

