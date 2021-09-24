---
title: FirstOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FirstOccurrence
api_type:
- schema
ms.assetid: d6748860-ce0d-4d2e-b7e4-9ed834f1e45a
description: FirstOccurrence 要素は、定期的な予定表アイテムの最初の出現を表します。
ms.openlocfilehash: e774e69f658479b1faab04eb9b91a2d24180e515
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518394"
---
# <a name="firstoccurrence"></a>FirstOccurrence

**FirstOccurrence** 要素は、定期的な予定表アイテムの最初の出現を表します。 
  
```xml
<FirstOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</FirstOccurrence>
```

 **OccurrenceInfoType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |定期的な予定表アイテムの最初の出現の一意の識別子と変更キーを含む。  <br/> |
|[Start](start.md) <br/> |定期的な予定表アイテムの最初の出現時刻を表します。  <br/> |
|[終わり ](end-ex15websvcsotherref.md) <br/> |定期的な予定表アイテムの最初の出現の終了時刻を表します。  <br/> |
|[OriginalStart](originalstart.md) <br/> |定期的な予定表アイテムの最初の出現の元の開始時刻を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は [、CalendarItemType に RecurringMaster](calendaritemtype.md) 値がある場合に有効です。 
  
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
  
[Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)

