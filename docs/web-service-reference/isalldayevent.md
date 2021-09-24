---
title: IsAllDayEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsAllDayEvent
api_type:
- schema
ms.assetid: 29140a64-9d7a-4a14-a10d-c98197c9831b
description: IsAllDayEvent 要素は、予定表アイテムまたは会議出席依頼が 1 日のイベントを表すかどうかを示します。
ms.openlocfilehash: 6dd40851f09fc25ebc8141ad059d7c6c908e92a3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541015"
---
# <a name="isalldayevent"></a>IsAllDayEvent

**IsAllDayEvent** 要素は、予定表アイテムまたは会議出席依頼が 1 日のイベントを表すかどうかを示します。 
  
```xml
<IsAllDayEvent/>
```

 **Boolean**
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
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素が含まれている場合は、ブール値を表すテキスト値が必要です。 値 true は **、** アイテムが 1 日のイベントを表すかどうかを示します。 false の **値は** 、アイテムがユーザーの作業時間より少ない範囲を示します。 
  
## <a name="remarks"></a>注釈

1 日のイベントは、メールボックスに対して定義されている勤務時間の期間にまたがっています。
  
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

