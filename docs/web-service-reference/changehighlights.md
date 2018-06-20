---
title: ChangeHighlights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: 要素は、会議の 2 つのバージョン間で変更内容を指定します。 ChangeHighlights は、メッセージを要求します。
ms.openlocfilehash: 5fe7aa95f60ae95f1af24e8f7a0463ad49716f65
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759617"
---
# <a name="changehighlights"></a>ChangeHighlights

**ChangeHighlights**要素で指定して、会議の 2 つのバージョン間での変更は、要求メッセージです。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[HasLocationChanged](haslocationchanged.md) <br/> |会議の場所のプロパティが変更されたかどうかを指定します。  <br/> |
|[場所](location.md) <br/> |会議または予定の場所を表します。  <br/> |
|[HasStartTimeChanged](hasstarttimechanged.md) <br/> |会議の開始時刻が変更されたかどうかを指定します。  <br/> |
|[Start](start.md) <br/> |期間の開始を表します。  <br/> |
|[HasEndTimeChanged](hasendtimechanged.md) <br/> |会議の終了時刻が変更されたかどうかを指定します。  <br/> |
|[終わり](end-ex15websvcsotherref.md) <br/> |期間の終了を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

