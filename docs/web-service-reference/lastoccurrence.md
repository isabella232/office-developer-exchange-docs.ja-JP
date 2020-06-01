---
title: LastOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LastOccurrence
api_type:
- schema
ms.assetid: c9ef0fcb-4265-4e60-9986-fff0f211d00b
description: LastOccurrence 要素は、定期的な予定表アイテムの最後の発生を表します。
ms.openlocfilehash: 8771bbed166cfb6fdcf4d1dfe4fa0812013e2667
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459813"
---
# <a name="lastoccurrence"></a>LastOccurrence

**Lastoccurrence**要素は、定期的な予定表アイテムの最後の発生を表します。 
  
```xml
<LastOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</LastOccurrence>
```

 **OccurrenceInfoType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |定期的な予定表アイテムの最後の発生の一意識別子および変更キーが含まれています。  <br/> |
|[開始](start.md) <br/> |定期的な予定表アイテムの最後の発生の開始時刻を表します。  <br/> |
|[終わり](end-ex15websvcsotherref.md) <br/> |定期的な予定表アイテムの最後の発生の終了時刻を表します。  <br/> |
|[OriginalStart](originalstart.md) <br/> |定期的な予定表アイテムが最後に発生したときの元の開始時刻を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
   
## <a name="remarks"></a>注釈

[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
  
[Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)

