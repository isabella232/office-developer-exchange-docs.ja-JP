---
title: オフセット
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Offset
api_type:
- schema
ms.assetid: dcbb9d85-d90c-4363-b4c9-d081ad03f407
description: オフセット要素は、BaseOffset からのオフセットを示します。 BaseOffset 要素とは、オフセット要素は、時間が標準または夏時間から標準時であるかどうかを識別します。
ms.openlocfilehash: d85fef0d67633733f6aa1943d70413ea70a528d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832642"
---
# <a name="offset"></a>オフセット

**オフセット**要素は、 [BaseOffset](baseoffset.md)からのオフセットを示します。 **BaseOffset**要素と要素の**オフセット**は、時間が標準または夏時間から標準時であるかどうかを識別します。 
  
```xml
<Offset/>
```

 **duration**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[(夏時間)](daylight.md) <br/> |日付と時刻が変更されたとき夏時間から標準時間への時間を表します。  <br/> |
|[Standard](standard.md) <br/> |日付と時刻が変更されたとき夏時間から標準時間への時間を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、世界協定時刻 (UTC) からのオフセットを表します。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

