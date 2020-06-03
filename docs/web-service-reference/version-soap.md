---
title: バージョン (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 47c9216e-6bfe-48c8-a27a-26f70db8e8d5
description: Version 要素は、サーバー製品バージョンの説明を表します。
ms.openlocfilehash: d7e6983c837b2818b7d11e1777015ec583968242
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44531029"
---
# <a name="version-soap"></a>バージョン (SOAP)

**Version**要素は、サーバー製品バージョンの説明を表します。 
  
```XML
<Version/>
```

 **string**
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

**Version**要素の値は、サーバー製品のバージョンの説明です。 
  
## <a name="remarks"></a>注釈

**Version**要素は、応答の SOAP ヘッダーに含まれています。 
  
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

