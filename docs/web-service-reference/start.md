---
title: 開始
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Start
api_type:
- schema
ms.assetid: 7cfe9979-c893-4f9b-b3a1-8f9e17515a4b
description: 開始要素では、期間の開始を表します。
ms.openlocfilehash: 8d013990e650b497abfa947938a69eed3fed7474
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833545"
---
# <a name="start"></a>開始

**開始**要素では、期間の開始を表します。 
  
```xml
<Start/>
```

**DateTime**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[DeletedOccurrence](deletedoccurrence.md) <br/> |定期的な予定表アイテムの削除済みアイテムを表します。  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |定期的な予定表アイテムが最初に見つかった位置を表します。  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |定期的な予定表アイテムが最後に見つかった位置を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[出現](occurrence.md) <br/> |定期的な予定表アイテムの 1 つの変更されたアイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、期間の開始を表します。
  
## <a name="remarks"></a>備考

UpdateItem 操作は、Exchange ストアの項目の[開始](start.md)と[終了](end-ex15websvcsotherref.md)時間を設定できます。 UpdateItem 要求では、[**終了**時刻を設定せず、**開始**時刻を設定できます。 **開始**時刻は**終了**時刻より後の場合は、エラーが発生することができます。 クライアント アプリケーションが**終了**時刻の期間を保持するために、その**開始**時間が変更されたときに調整を行う必要があることに注意します。 
  
> [!NOTE]
> 定期的なマスター アイテムの[開始](start.md)と[終了](end-ex15websvcsotherref.md)日が毎週の定期的なパターンの 1 番目の日付があるない場合、タイム ゾーン オフセット情報は失われます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [WeeklyRecurrence](weeklyrecurrence.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

