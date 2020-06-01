---
title: FreeBusyView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: FreeBusyView 要素には、特定のユーザーの空き時間情報が含まれています。
ms.openlocfilehash: e5cc3bea6b57d5c400dd9be44bf9f9aaf9e43eb9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456102"
---
# <a name="freebusyview"></a>FreeBusyView

**FreeBusyView**要素には、特定のユーザーの空き時間情報が含まれています。 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
```xml
<FreeBusyView>
   <FreeBusyViewType>...</FreeBusyViewType>
   <MergedFreeBusy>...</MergedFreeBusy>
   <CalendarEventArray>...</CalendarEventArray>
   <WorkingHours>...</WorkingHours>
</FreeBusyView>
```

 **FreeBusyView**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FreeBusyViewType](freebusyviewtype.md) <br/> |応答で返される要求された空き時間情報の種類を表します。  <br/> |
|[MergedFreeBusy](mergedfreebusy.md) <br/> |データのマージされた空き時間ストリームを格納します。  <br/> |
|[CalendarEventArray](calendareventarray.md) <br/> |要求されたユーザーの空き時間情報を表す、一連の一意な予定表アイテムの繰り返しを含みます。  <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |要求されたメールボックスユーザーのタイムゾーン設定および稼働時間を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FreeBusyResponse](freebusyresponse.md) <br/> |1つのメールボックスユーザーの空き時間情報が含まれています。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a>注釈

すべての子要素が発生する順序で一覧表示されます。 この要素によって提供される詳細レベルは、リクエスターに付与されるアクセス許可によって異なります。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[ユーザーの空き時間情報の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

