---
title: Offset
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
description: Offset 要素は、BaseOffset からのオフセットを表します。 BaseOffset 要素と共に、Offset 要素は時刻が標準時であるか夏時間であるかを識別します。
ms.openlocfilehash: 74ad87026c2cb89f3b0c35218c91f81380029963
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459757"
---
# <a name="offset"></a>Offset

**Offset**要素は、 [baseoffset](baseoffset.md)からのオフセットを表します。 **Baseoffset**要素と共に、 **Offset**要素は時刻が標準時であるか夏時間であるかを識別します。 
  
```xml
<Offset/>
```

 **duration**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[日光](daylight.md) <br/> |夏時間から標準時までの時刻が変更された日付と時刻を表します。  <br/> |
|[Standard](standard.md) <br/> |夏時間から標準時までの時刻が変更された日付と時刻を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、協定世界時 (UTC) からのオフセットを表します。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

