---
title: DaysOfWeek (DayOfWeekType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaysOfWeek
api_type:
- schema
ms.assetid: ba8f990d-d37d-403d-b31f-55e5208c8ad5
description: DaysOfWeek 要素では、項目の定期的なパターンで使用されている週の日について説明します。
ms.openlocfilehash: a7afb0aeb650284739d559164f06590fc5266c57
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/21/2018
ms.locfileid: "19759946"
---
# <a name="daysofweek-dayofweektype"></a>DaysOfWeek (DayOfWeekType)

**DaysOfWeek**要素では、項目の定期的なパターンで使用されている週の日について説明します。 
  
```xml
<DaysOfWeek/>
```

**DayOfWeekType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |相対年間の定期的なパターンをについて説明します。  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |相対的な毎月の定期的なパターンをについて説明します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 指定可能な値は次のいずれかです。
  
- 日曜日    
- 月曜日    
- 火曜日   
- 水曜日    
- 木曜日    
- 金曜日    
- 土曜日    
- (、TimeChangePatternTypes では使用されません) の日    
- (、TimeChangePatternTypes では使用されません) の平日    
- (、TimeChangePatternTypes では使用されません) WeekendDay
    
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

