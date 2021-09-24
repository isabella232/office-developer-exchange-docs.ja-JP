---
title: Daylight
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Daylight
api_type:
- schema
ms.assetid: ea400839-fba8-4a5e-a5d1-9b677afc0ff9
description: Daylight 要素は、時刻が標準時から夏時間に変更される日時を表します。
ms.openlocfilehash: 750d7cb97d9e2967d3477a93ae833229d20619dc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517218"
---
# <a name="daylight"></a>Daylight

**Daylight 要素** は、時刻が標準時から夏時間に変更される日時を表します。 
  
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
|**TimeZoneName** <br/> |タイム ゾーンの名前を説明します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Offset](offset.md) <br/> |BaseOffset からのオフセット [について説明します](baseoffset.md)。 このオフセットに加えて基本オフセットは、標準時か夏時間かに応じて時刻を識別します。  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |タイム ゾーン移行日パターンの相対的な年次定期的なパターンを説明します。  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |標準または夏時間から時刻が変更される日付を表します。  <br/> |
|[Time (TimeChangeType)](time-timechangetype.md) <br/> |標準時と夏時間の間で時刻が変化する時刻を示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingTimeZone](meetingtimezone.md) <br/> |会議がホストされている場所のタイム ゾーンを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

