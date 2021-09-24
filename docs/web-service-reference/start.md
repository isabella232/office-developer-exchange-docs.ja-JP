---
title: 開始
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Start
api_type:
- schema
ms.assetid: 7cfe9979-c893-4f9b-b3a1-8f9e17515a4b
description: Start 要素は、期間の開始を表します。
ms.openlocfilehash: 7342e285e57a165ec4a9ba0b8551bfbe045d3b9c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521271"
---
# <a name="start"></a>開始

**Start 要素** は、期間の開始を表します。 
  
```xml
<Start/>
```

**DateTime**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[DeletedOccurrence](deletedoccurrence.md) <br/> |定期的な予定表アイテムの削除済みアイテムを表します。  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |定期的な予定表アイテムの最初の出現を表します。  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |定期的な予定表アイテムの最後の出現を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
|[Occurrence](occurrence.md) <br/> |定期的な予定表アイテムが 1 回変更された場合を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、期間の開始を表します。
  
## <a name="remarks"></a>注釈

UpdateItem 操作では、ストア アイテム[](end-ex15websvcsotherref.md)[の開始](start.md)時刻と終了時刻Exchange設定できます。 UpdateItem 要求では、終了時刻も設定せずに開始時刻を **設定** できます。 開始時刻が終了時刻より後の場合、エラーが **発生する可能性** があります。 クライアント アプリケーションは、期間を保持するために開始時刻が変更された場合に終了時刻に調整を実行する必要があります。 
  
> [!NOTE]
> タイム ゾーン のオフセット情報は、[](start.md)定期的な[](end-ex15websvcsotherref.md)マスター アイテムの開始日と終了日に、週ごとの定期的なパターンの最初の出現日付と等しくない場合に失われます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [WeeklyRecurrence](weeklyrecurrence.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

