---
title: Standard
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
description: 標準的な要素では、日付と時刻が変更されたとき夏時間から標準時間への時間を表します。
ms.openlocfilehash: c121e959f243d982cfe50ed6b4ef39a82dae2cc8
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353435"
---
# <a name="standard"></a>Standard

**標準的な**要素では、日付と時刻が変更されたとき夏時間から標準時間への時間を表します。 
  
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**TimeZoneName** <br/> |タイム ゾーンの名前について説明します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Offset](offset.md) <br/> |[BaseOffset](baseoffset.md)からのオフセットを示します。 **BaseOffset**要素とは、**オフセット**要素は、時間が標準時か夏時間かどうかを識別します。  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |タイム ゾーンの移行日の相対的な年間の定期的なパターンを説明します。  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |標準時間または夏時間から標準時から時間が変更されたときの日付を表します。  <br/> |
|[Time (TimeChangeType)](time-timechangetype.md) <br/> |標準時と夏時間との間の時間が変更されたときの時間について説明します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingTimeZone](meetingtimezone.md) <br/> |会議がホストされている場所のタイム ゾーンを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

