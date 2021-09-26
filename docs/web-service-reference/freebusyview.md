---
title: FreeBusyView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: FreeBusyView 要素には、特定のユーザーの可用性情報が含まれる。
ms.openlocfilehash: c662e8a44118f61b4c8be642d9ac862051c3a15d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546414"
---
# <a name="freebusyview"></a>FreeBusyView

**FreeBusyView 要素** には、特定のユーザーの可用性情報が含まれる。 
  
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
|[MergedFreeBusy](mergedfreebusy.md) <br/> |データの結合された空き時間情報ストリームが含まれます。  <br/> |
|[CalendarEventArray](calendareventarray.md) <br/> |要求されたユーザーの可用性を表す一意の予定表アイテムの出現のセットを含みます。  <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |要求されたメールボックス ユーザーのタイム ゾーン設定と作業時間を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FreeBusyResponse](freebusyresponse.md) <br/> |単一のメールボックス ユーザーの空き時間情報が含まれる。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a>注釈

すべての子要素は、その子要素が発生する順序で一覧表示されます。 この要素によって提供される詳細レベルは、要求者に付与されるアクセス許可によって異なります。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

