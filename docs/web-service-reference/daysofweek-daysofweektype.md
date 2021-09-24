---
title: DaysOfWeek (DaysOfWeekType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DaysOfWeek
api_type:
- schema
ms.assetid: c56f997d-28f3-4590-97b0-cb71f016dbe4
description: DaysOfWeek 要素は、アイテムの定期的なパターンで使用される週の日数を表します。
ms.openlocfilehash: 9b0786149f943c47ab77bcb69b74542cbc08edd5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519871"
---
# <a name="daysofweek-daysofweektype"></a>DaysOfWeek (DaysOfWeekType)

**DaysOfWeek 要素** は、アイテムの定期的なパターンで使用される週の日数を表します。 
  
```XML
<DaysOfWeek/>
```

**DaysOfWeekType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |毎週の定期的なパターンについて説明します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 指定可能な値は次のいずれかです。
  
- 日曜日    
- 月曜日    
- 火曜日    
- 水曜日    
- 木曜日    
- 金曜日    
- 土曜日    
- Day (この値は週単位の定期的なパターンでは無効です)    
- 平日 (この値は週単位の定期的なパターンでは無効です)    
- WeekendDay (この値は週単位の定期的なパターンでは無効)
    
毎週の定期的なパターンには、複数の値を含めることができます。 値はスペース文字で区切ります。 たとえば、火曜日と木曜日の毎週の繰り返しの場合、テキスト値は "火曜日の木曜日" になります。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

