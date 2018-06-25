---
title: 終了
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- End
api_type:
- schema
ms.assetid: 72329821-32ff-495d-b6e5-fdc011003c2e
description: 末尾の要素は、期間の終了を表します。
ms.openlocfilehash: 90eea4fc545fae083e5675225665e517b502ba6f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760284"
---
# <a name="end"></a>終了

**末尾**の要素は、期間の終了を表します。 
  
```xml
<End/>
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
|[FirstOccurrence](firstoccurrence.md) <br/> |定期的な予定表アイテムが最初に見つかった位置を表します。  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |定期的な予定表アイテムが最後に見つかった位置を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[出現](occurrence.md) <br/> |定期的な予定表アイテムの 1 つの変更されたアイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、期間の終了を表します。
  
## <a name="remarks"></a>備考

UpdateItem 操作は、Exchange ストアの項目の[開始](start.md)と**終了**時間を設定できます。 UpdateItem 要求では、**終了**時刻を設定せず、[開始](start.md)時刻を設定できます。 [開始](start.md)時刻は**終了**時刻より後の場合は、エラーが発生することができます。 クライアント アプリケーションが、期間を保持するために[開始](start.md)時間を変更するときの**終了**時刻の調整を行う必要があることに注意します。 
  
 **メモ**定期的なマスター アイテムの[開始](start.md)と**終了**日が毎週の定期的なパターンの 1 番目の日付があるない場合、タイム ゾーン オフセット情報は失われます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[WeeklyRecurrence](weeklyrecurrence.md)
  
 **End**


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

