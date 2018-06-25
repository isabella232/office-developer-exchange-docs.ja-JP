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
description: ピリオド要素は、タイム ゾーンの特定の段階の名前、時間のオフセット、および一意の識別子を定義します。
ms.openlocfilehash: 3b5d5877e6d9baffdfe536a0feec3b25b6d2883f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832726"
---
# <a name="period"></a>ピリオド

**期間**要素は、タイム ゾーンの特定の段階の名前、時間のオフセット、および一意の識別子を定義します。 
  
```xml
<Period Bias="" Name="" Id=""/>
```

 **PeriodType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|Bias  <br/> |期間の世界協定時刻 (UTC) からの時間のオフセットを表す文字列型 (xs:duration) の値を指定します。  <br/> |
|名前  <br/> |期間のわかりやすい名前を表す文字列値です。  <br/> |
|ID  <br/> |期間の識別子を表す文字列値。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Periods](periods.md) <br/> |タイム ゾーンのさまざまな段階での時刻のオフセットを定義する期間の配列を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

