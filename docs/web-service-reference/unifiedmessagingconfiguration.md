---
title: UnifiedMessagingConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnifiedMessagingConfiguration
api_type:
- schema
ms.assetid: cbdb4268-077e-44ed-8ec2-9d759c84cc6d
description: UnifiedMessagingConfiguration 要素には、ユニファイドメッセージングサービスのサービス構成情報が含まれています。
ms.openlocfilehash: 3f9f4ed65721929c552615c07e2239f48ef837f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528693"
---
# <a name="unifiedmessagingconfiguration"></a>UnifiedMessagingConfiguration

**UnifiedMessagingConfiguration**要素には、ユニファイドメッセージングサービスのサービス構成情報が含まれています。 
  
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
|[UmEnabled](umenabled.md) <br/> |アカウントに対してユニファイドメッセージングが有効になっているかどうかを示します。 この要素は必須です。  <br/> |
|[PlayOnPhoneDialString (Exchange Web サービス)](playonphonedialstring-exchange-web-services.md) <br/> |電話での通話のダイヤル文字列を識別します。 この要素は必須です。  <br/> |
|[Playon電話有効](playonphoneenabled.md) <br/> |電話での再生機能が有効になっているかどうかを示します。 この要素は必須です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |サービス構成の設定が含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
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

