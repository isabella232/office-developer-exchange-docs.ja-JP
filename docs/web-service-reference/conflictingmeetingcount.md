---
title: ConflictingMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConflictingMeetingCount
api_type:
- schema
ms.assetid: 11f4d93a-b514-4a27-8d19-f4f0a35a185e
description: ConflictingMeetingCount 要素は、予定表アイテムと競合する会議の数を表します。
ms.openlocfilehash: e6929160dacdf026ba8551bbcf6f991fbdc0b909
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536883"
---
# <a name="conflictingmeetingcount"></a>ConflictingMeetingCount

**ConflictingMeetingCount** 要素は、予定表アイテムと競合する会議の数を表します。 
  
```xml
<ConflictingMeetingCount/>
```

 **int**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議Exchangeします。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は整数を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。
  
## <a name="remarks"></a>注釈

予定表アイテムは、少なくとも部分的に、同じ予定表フォルダー内の別の予定表アイテムと同時に発生した場合、競合と見なされます。 予定表アイテムが非カレンダー フォルダーにある場合は、既定の予定表フォルダー内の予定表アイテムと比較されます。 会議出席依頼は、既定の予定表フォルダー内の予定表アイテムと比較されます。
  
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

