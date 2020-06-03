---
title: ChangeHighlights 強調表示
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: ChangeHighlights 要素は、2つのバージョンの会議出席依頼メッセージの間で変更されたものを指定します。
ms.openlocfilehash: 6c78d2c96449ee41032859f90bf51d6e0faa92ae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463280"
---
# <a name="changehighlights"></a>ChangeHighlights 強調表示

**Changehighlights**要素は、2つのバージョンの会議出席依頼メッセージの間で変更されたものを指定します。 
  
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
|[場所](location.md) <br/> |会議または予定の場所を表します。  <br/> |
|[HasStartTimeChanged](hasstarttimechanged.md) <br/> |会議の開始時刻が変更されたかどうかを指定します。  <br/> |
|[開始](start.md) <br/> |期間の開始を表します。  <br/> |
|[HasEndTimeChanged](hasendtimechanged.md) <br/> |会議の終了時刻が変更されたかどうかを指定します。  <br/> |
|[終わり](end-ex15websvcsotherref.md) <br/> |期間の最後の部分を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

