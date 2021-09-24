---
title: EndTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EndTimeZone
api_type:
- schema
ms.assetid: 6c53c337-be60-4d22-9e9e-a0c140c5e913
description: EndTimeZone 要素は、CalendarItem または MeetingRequest の終了時刻のタイム ゾーンを定義します。
ms.openlocfilehash: 6d34afdedfb8e4886526317afea6abc324bde3c8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520697"
---
# <a name="endtimezone"></a>EndTimeZone

**EndTimeZone** 要素は [、CalendarItem](calendaritem.md)または MeetingRequest の終了時刻のタイム ゾーン [を定義します](meetingrequest.md)。
  
```xml
<EndTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</EndTimeZone>
```

 **TimeZoneDefinitionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |タイム ゾーン定義の一意の識別子を表します。  <br/> |
|名前  <br/> |タイム ゾーン定義のわかりやすい名前を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Periods](periods.md) <br/> |タイム ゾーンの異なるステージでのタイム オフセットを定義する [Period](period.md) 要素の配列を表します。  <br/> |
|[TransitionsGroups](transitionsgroups.md) <br/> |タイム ゾーンの遷移を [指定する TransitionsGroup](transitionsgroup.md) 要素の配列を表します。  <br/> |
|[Transitions](transitions.md) <br/> |タイム ゾーン遷移の配列を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Microsoft Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

