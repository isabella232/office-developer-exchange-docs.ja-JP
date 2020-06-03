---
title: Time (TimeChangeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Time
api_type:
- schema
ms.assetid: be12e41e-6871-4f6b-b2d4-3dfa404f9ea1
description: Time 要素は、標準時と夏時間の間で時刻が変更された時刻を表します。
ms.openlocfilehash: c25d0bc3394fdfab42a29eab8b370bc4263618ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465738"
---
# <a name="time-timechangetype"></a>Time (TimeChangeType)

**Time**要素は、標準時と夏時間の間で時刻が変更された時刻を表します。 
  
```xml
<Time/>
```

 **Time**
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

Text 値は、標準時と夏時間の間で時刻が変更された時刻を表します。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

