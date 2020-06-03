---
title: MajorBuildNumber (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7335b1c1-0b47-4452-a8cb-d19cddcfc281
description: MajorBuildNumber 要素は、サーバーの主要なビルド番号を表します。
ms.openlocfilehash: 60a8cbeb4b689da85bbb72c2d93759799b913f2f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465885"
---
# <a name="majorbuildnumber-soap"></a>MajorBuildNumber (SOAP)

**MajorBuildNumber**要素は、サーバーの主要なビルド番号を表します。 
  
```XML
<MajorBuildNumber/>
```

 **xs: int**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ServerVersionInfo (SOAP)](serverversioninfo-soap.md) <br/> |要求を処理したサーバーのバージョンが保存されています。  <br/> |
   
## <a name="text-value"></a>テキスト値

MajorBuildNumber 要素のテキスト値は、要求を処理したサーバーのメジャービルド番号を表す整数型 (integer) の値です。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
  
[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)
  
[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)

