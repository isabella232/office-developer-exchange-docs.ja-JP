---
title: サポートされている apiversion
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d9264e74-eba7-4279-b193-af7e5130268d
description: ApiVersionSupported 要素には、クライアントでサポートされている JavaScript API for Office のバージョンが含まれています。
ms.openlocfilehash: 0129a33624b48d309ad0814af6eaa655b2c4e6f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466060"
---
# <a name="apiversionsupported"></a>サポートされている apiversion

**Apiversionsupported**要素には、クライアントでサポートされている JavaScript API for Office のバージョンが含まれています。 
  
```XML
<ApiVersionSupported />
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Getappmanifests が](getappmanifests.md)
  
## <a name="text-value"></a>テキスト値

**Apiversionsupported**要素のテキスト値には、クライアントでサポートされている JavaScript API for Office のバージョンが含まれています。 この値は、応答でクライアントに返されるアプリケーションマニフェストを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> | https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |該当なし  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Getappmanifests が](getappmanifests.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

