---
title: ApiVersionSupported
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d9264e74-eba7-4279-b193-af7e5130268d
description: ApiVersionSupported 要素には、JavaScript API のクライアントでサポートされている Office のバージョンが含まれています。
ms.openlocfilehash: 41c3eacff65d797dfe7e8b587c50c35d8938664f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759326"
---
# <a name="apiversionsupported"></a>ApiVersionSupported

**ApiVersionSupported**要素には、JavaScript API のクライアントでサポートされている Office のバージョンが含まれています。 
  
```XML
<ApiVersionSupported />
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[GetAppManifests](getappmanifests.md)
  
## <a name="text-value"></a>テキスト値

**ApiVersionSupported**要素のテキスト値には、JavaScript API のクライアントでサポートされている Office のバージョンが含まれています。 この値は、アプリケーション マニフェストは、応答でクライアントに返される必要がありますを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> | http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |該当しない  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetAppManifests](getappmanifests.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

