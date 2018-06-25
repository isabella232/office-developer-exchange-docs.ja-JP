---
title: NoEndRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NoEndRecurrence
api_type:
- schema
ms.assetid: ab2ebd9c-388e-45f1-abf9-56e293ef123b
description: NoEndRecurrence 要素は、定義された終了日がない項目の定期的なパターンの開始日について説明します。
ms.openlocfilehash: fc3eae170f5c07e31d7a80b45836efd07d74e543
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832537"
---
# <a name="noendrecurrence"></a>NoEndRecurrence

**NoEndRecurrence**要素は、定義された終了日がない項目の定期的なパターンの開始日について説明します。 
  
```xml
<NoEndRecurrence>
   <StartDate/>
</NoEndRecurrence>
```

 **NoEndRecurrenceRangeType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[開始日 (繰り返し)](startdate-recurrence.md) <br/> |定期的な仕事または予定表アイテムの開始日を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[定期的なアイテム (RecurrenceType)](recurrence-recurrencetype.md) <br/> |予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。  <br/> |
|[定期的な予定 (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |定期タスクの頻度に関する情報が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

