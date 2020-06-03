---
title: 標準
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Standard
api_type:
- schema
ms.assetid: d598f0a6-e296-423f-8ce5-3da57cfd8189
description: Standard 要素は、夏時間から標準時に時刻が変更された日付と時刻を表します。
ms.openlocfilehash: 1214a1debb53c9a31ca7c92a0c9e5c0722960d75
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467565"
---
# <a name="standard"></a>標準

**Standard**要素は、夏時間から標準時に時刻が変更された日付と時刻を表します。 
  
```xml
<Standard TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Standard>
```

```xml
<Standard TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Standard>
```

**TimeChangeType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**TimeZoneName** <br/> |タイムゾーンの名前を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Offset](offset.md) <br/> |[Baseoffset](baseoffset.md)からのオフセットを記述します。 **Baseoffset**要素と共に、 **Offset**要素は時刻が標準時であるか夏時間であるかを識別します。  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |タイムゾーンの移行日の相対的な年単位のパターンを記述します。  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |標準時または夏時間から時刻が変更された日付を表します。  <br/> |
|[Time (TimeChangeType)](time-timechangetype.md) <br/> |時刻が標準時と夏時間の間に変化する時間を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingTimeZone](meetingtimezone.md) <br/> |会議がホストされている場所のタイムゾーンを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

