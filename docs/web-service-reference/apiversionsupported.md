---
title: ApiVersionSupported
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d9264e74-eba7-4279-b193-af7e5130268d
description: ApiVersionSupported 要素には、クライアントがサポートする JavaScript API Officeが含まれている。
ms.openlocfilehash: 4b3034e05e294564b73d99f706d325d7d75b4f88
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543716"
---
# <a name="apiversionsupported"></a>ApiVersionSupported

**ApiVersionSupported 要素** には、クライアントでサポートされている JavaScript API Officeが含まれている。 
  
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

[GetAppManifests](getappmanifests.md)
  
## <a name="text-value"></a>テキスト値

**ApiVersionSupported** 要素のテキスト値には、クライアントでサポートされている JavaScript API Officeが含まれている。 この値は、応答でクライアントに返すアプリ マニフェストを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> | https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |該当なし  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetAppManifests](getappmanifests.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

