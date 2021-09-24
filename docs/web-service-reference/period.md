---
title: Period
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Period
api_type:
- schema
ms.assetid: 2f9cf6af-c531-4d7d-90c9-1a1db504d890
description: Period 要素は、タイム ゾーンの特定のステージの名前、タイム オフセット、および一意の識別子を定義します。
ms.openlocfilehash: 7fa5bca6547f4e3120c60c2e2b69139f7bb12e93
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534736"
---
# <a name="period"></a>Period

**Period 要素** は、タイム ゾーンの特定のステージの名前、タイム オフセット、および一意の識別子を定義します。 
  
```xml
<Period Bias="" Name="" Id=""/>
```

 **PeriodType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|Bias  <br/> |期間の協定世界時 (UTC) からの時間オフセットを表す xs:duration 値。  <br/> |
|名前  <br/> |ピリオドのわかりやすい名前を表す文字列値。  <br/> |
|ID  <br/> |期間の識別子を表す文字列値。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Periods](periods.md) <br/> |タイム ゾーンの異なるステージでのタイム オフセットを定義する期間の配列を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

