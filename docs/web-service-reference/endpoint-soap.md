---
title: エンドポイント (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 630cdbb5-d1c7-422c-924a-abf5738e9e5e
description: エンドポイント要素は、セキュリティ トークン サービスのエンドポイントを指定します。
ms.openlocfilehash: 85e1ad785b35649238ac3944f51472addf617c20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760295"
---
# <a name="endpoint-soap"></a>エンドポイント (SOAP)

**エンドポイント**要素は、セキュリティ トークン サービスのエンドポイントを指定します。 
  
```XML
<Endpoint/>
```

 **xs:anyURI**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

なし
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |セキュリティ トークン サービスの URI のエンドポイントを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、セキュリティ トークンの web サービスのエンドポイントを表します。
  
## <a name="remarks"></a>備考

エンドポイントは、セキュリティ トークンの web サービスと通信するために使用されます。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   

