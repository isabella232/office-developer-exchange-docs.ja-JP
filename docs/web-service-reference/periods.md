---
title: 期間
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Periods
api_type:
- schema
ms.assetid: 7920d81d-abba-4232-8bfe-49267b6c9a36
description: ピリオド要素では、タイム ゾーンのさまざまな段階での時刻のオフセットを定義する期間の配列を表します。
ms.openlocfilehash: f2f9cf7c724b453d2b1975fcf72c55bc02caa54b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832729"
---
# <a name="periods"></a>期間

**ピリオド**要素では、タイム ゾーンのさまざまな段階での時刻のオフセットを定義する期間の配列を表します。 
  
```xml
<Periods>
   <Period/>
</Periods>
```

 **NonEmptyArrayOfPeriodsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Period](period.md) <br/> |タイム ゾーンの特定の段階の名前、時間のオフセット、および一意の識別子を定義します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StartTimeZone](starttimezone.md) <br/> |[カレンダー項目](calendaritem.md)または[MeetingRequest](meetingrequest.md)の開始時刻のタイム ゾーンを定義します。  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |[カレンダー項目](calendaritem.md)または[MeetingRequest](meetingrequest.md)の終了時刻のタイム ゾーンを定義します。  <br/> |
|[タイム](timezonedefinition.md) <br/> |タイム ゾーンを定義します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

