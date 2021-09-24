---
title: SchemaVersionSupported
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 578b1682-f3e1-4ccc-aa24-d2ca1a9de596
description: SchemaVersionSupported 要素には、クライアントでサポートされているマニフェスト スキーマのバージョンが含まれています。
ms.openlocfilehash: 289631467499bdc0c80e1572ce43202153f2103c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515216"
---
# <a name="schemaversionsupported"></a>SchemaVersionSupported

**SchemaVersionSupported 要素** には、クライアントでサポートされているマニフェスト スキーマのバージョンが含まれています。 
  
```XML
<SchemaVersionSupported />
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

**SchemaVersionSupported** 要素のテキスト値には、クライアントでサポートされているマニフェスト スキーマのバージョンが含まれています。 この値は、応答でクライアントに返すアプリ マニフェストを示します。 
  
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



[GetAppManifests](getappmanifests.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

