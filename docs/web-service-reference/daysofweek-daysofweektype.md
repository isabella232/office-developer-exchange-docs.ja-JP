---
title: DaysOfWeek (DaysOfWeekType)
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
ms.assetid: c56f997d-28f3-4590-97b0-cb71f016dbe4
description: DaysOfWeek 要素では、項目の定期的なパターンで使用されている週の日について説明します。
ms.openlocfilehash: 0b730ff5a7bc9aa6b324fc080022d056c5342296
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759945"
---
# <a name="daysofweek-daysofweektype"></a>DaysOfWeek (DaysOfWeekType)

**DaysOfWeek**要素では、項目の定期的なパターンで使用されている週の日について説明します。 
  
```XML
<DaysOfWeek/>
```

**DaysOfWeekType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |毎週の定期的なパターンをについて説明します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 指定可能な値は次のいずれかです。
  
- 日曜日    
- 月曜日    
- 火曜日    
- 水曜日    
- 木曜日    
- 金曜日    
- 土曜日    
- (この値は毎週の定期的なパターンに対して有効ではありません) の日    
- (この値は毎週の定期的なパターンに対して有効ではありません) の平日    
- (この値は毎週の定期的なパターンに対して有効ではありません) WeekendDay
    
毎週の定期的なパターンでは、複数の値を含めることができます。 値は、空白文字で区切られます。 たとえば、火曜日と木曜日の毎週、テキスト値に「火曜日木曜日」です。
  
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

