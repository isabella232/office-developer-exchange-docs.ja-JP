---
title: ピリオド
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Period
api_type:
- schema
ms.assetid: 2f9cf6af-c531-4d7d-90c9-1a1db504d890
description: Period 要素は、タイムゾーンの特定のステージの名前、時刻オフセット、および一意識別子を定義します。
ms.openlocfilehash: a7c36a9de01fd0484a7df75de3b5525992ef7ee7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459722"
---
# <a name="period"></a>ピリオド

**Period**要素は、タイムゾーンの特定のステージの名前、時刻オフセット、および一意識別子を定義します。 
  
```xml
<Period Bias="" Name="" Id=""/>
```

 **PeriodType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|バイアス  <br/> |期間の協定世界時 (UTC) からの時間オフセットを表す xs: duration 値。  <br/> |
|名前  <br/> |期間のわかりやすい名前を表す文字列型 (string) の値を指定します。  <br/> |
|ID  <br/> |期間の識別子を表す文字列型 (string) の値を指定します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Periods](periods.md) <br/> |タイムゾーンのさまざまな段階での時間オフセットを定義する期間の配列を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

