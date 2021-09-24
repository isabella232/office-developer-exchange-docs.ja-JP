---
title: ChangeHighlights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: ChangeHighlights 要素は、2 つのバージョンの会議出席依頼メッセージの間で何が変更されたかを指定します。
ms.openlocfilehash: 95f665f30c62d723cd97eaa2bd3eb3b2ed479967
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512213"
---
# <a name="changehighlights"></a>ChangeHighlights

**ChangeHighlights 要素** は、2 つのバージョンの会議出席依頼メッセージの間で何が変更されたかを指定します。 
  
```XML
<ChangeHighlights>
    <HasLocationChanged></HasLocationChanged>
    <Location></Location>
    <HasStartTimeChanged></HasStartTimeChanged>
    <Start></Start>
    <HasEndTimeChanged></HasEndTimeChanged>
    <End></End>
</ChangeHighlights>
```

 **ChangeHighlightsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[HasLocationChanged](haslocationchanged.md) <br/> |会議の場所プロパティが変更されたかどうかを指定します。  <br/> |
|[Location](location.md) <br/> |会議または予定の場所を表します。  <br/> |
|[HasStartTimeChanged](hasstarttimechanged.md) <br/> |会議の開始時刻が変更されたかどうかを指定します。  <br/> |
|[Start](start.md) <br/> |期間の開始を表します。  <br/> |
|[HasEndTimeChanged](hasendtimechanged.md) <br/> |会議の終了時刻が変更されたかどうかを指定します。  <br/> |
|[終わり ](end-ex15websvcsotherref.md) <br/> |期間の終了を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

