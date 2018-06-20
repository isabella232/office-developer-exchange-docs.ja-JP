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
description: FreeBusyView 要素には、特定のユーザーの利用可能時間情報が含まれています。
ms.openlocfilehash: d0d603f18642a94e841a1a6bb8e8849aa6b5b273
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760602"
---
# <a name="freebusyview"></a>FreeBusyView

**FreeBusyView**要素には、特定のユーザーの利用可能時間情報が含まれています。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FreeBusyViewType](freebusyviewtype.md) <br/> |要求された空き時間情報が応答で返されるの種類を表します。  <br/> |
|[MergedFreeBusy](mergedfreebusy.md) <br/> |結合された空き時間情報データ ストリームが含まれています。  <br/> |
|[CalendarEventArray](calendareventarray.md) <br/> |要求されたユーザーの可用性を表す一意の予定表アイテムの出現回数のセットが含まれています。  <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |要求されたメールボックスのユーザーの作業時間とタイム ゾーンの設定を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FreeBusyResponse](freebusyresponse.md) <br/> |1 つのメールボックスのユーザーの空き時間情報が含まれています。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a>備考

発生したシーケンスは、すべての子要素の一覧です。 この要素によって提供される詳細のレベルは、要求側に付与するアクセス許可に依存します。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

