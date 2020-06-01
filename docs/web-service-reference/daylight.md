---
title: 日光
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Daylight
api_type:
- schema
ms.assetid: ea400839-fba8-4a5e-a5d1-9b677afc0ff9
description: 夏時間要素は、時刻が標準時から夏時間に変更された日時を表します。
ms.openlocfilehash: bf2041cb4677f837ddb5b399041f1c19a7b5f577
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457460"
---
# <a name="daylight"></a>日光

**夏時間**要素は、時刻が標準時から夏時間に変更された日時を表します。 
  
```xml
<Daylight TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Daylight>
```

```xml
<Daylight TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Daylight>
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
|[Offset](offset.md) <br/> |[Baseoffset](baseoffset.md)からのオフセットを記述します。 このオフセットに加えてベースオフセットを指定すると、標準または夏時間であるかどうかに応じて時刻が識別されます。  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |タイムゾーンの移行日パターンに関する相対的な年単位のパターンを記述します。  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |時刻が標準または夏時間から変化する日付を表します。  <br/> |
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

