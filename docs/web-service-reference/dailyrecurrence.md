---
title: DailyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DailyRecurrence
api_type:
- schema
ms.assetid: 0aaf265d-b723-49c6-8e9c-9ba60141e9ab
description: DailyRecurrence 要素は、予定表アイテムまたはタスクが再帰する頻度を日数で表します。
ms.openlocfilehash: 7f79b4f69571a1d3ea1c661831825fb2899ebcdb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535942"
---
# <a name="dailyrecurrence"></a>DailyRecurrence

**DailyRecurrence** 要素は、予定表アイテムまたはタスクが再帰する頻度を日数で表します。 
  
```xml
<DailyRecurrence>
   <Interval/>
</DailyRecurrence>
```

**DailyRecurrencePatternType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[間隔](interval.md) <br/> |2 つの連続する定期的なアイテム間の間隔を日数で定義します。 値は 1 ~ 999 の範囲である必要があります。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Recurrence (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |定期的なタスクの定期的な情報が含まれています。  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |予定表アイテムと会議出席依頼の定期的なパターンが含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

