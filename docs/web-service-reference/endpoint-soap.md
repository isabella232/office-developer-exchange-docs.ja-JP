---
title: エンドポイント (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 630cdbb5-d1c7-422c-924a-abf5738e9e5e
description: Endpoint 要素は、security token service エンドポイントを指定します。
ms.openlocfilehash: 93659bbefa4a95063304cf3abad81cb61767070a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458398"
---
# <a name="endpoint-soap"></a>エンドポイント (SOAP)

**Endpoint**要素は、security token service エンドポイントを指定します。 
  
```XML
<Endpoint/>
```

 **xs: anyURI**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

なし
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |セキュリティトークンサービスの URI とエンドポイントを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、セキュリティトークン web サービスのエンドポイントを表します。
  
## <a name="remarks"></a>注釈

エンドポイントは、セキュリティトークン web サービスとの通信に使用されます。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |はい  <br/> |
   

