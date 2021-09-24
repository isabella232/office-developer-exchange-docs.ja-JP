---
title: MergedFreeBusy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MergedFreeBusy
api_type:
- schema
ms.assetid: ea45590d-476e-4b68-9fe8-ae392feadfea
description: MergedFreeBusy 要素には、結合されたデータの空き時間情報ストリームが含まれます。
ms.openlocfilehash: db451d6b2e67313836771604fae57b14b6b3db10
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511031"
---
# <a name="mergedfreebusy"></a>MergedFreeBusy

**MergedFreeBusy 要素には**、結合されたデータの空き時間情報ストリームが含まれます。 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[MergedFreeBusy](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FreeBusyView](freebusyview.md) <br/> |特定のユーザーの可用性情報が含まれる。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>テキスト値

[FreeBusyViewType](freebusyviewtype.md)要素の値が次のいずれかの場合、サーバーによってテキスト値が提供されます。 
  
- Detailedmerged
    
- FreeBusyMerged
    
- MergedOnly
    
テキスト値は、空き時間情報のストリームです。 
  
## <a name="remarks"></a>注釈

この要素によって提供されるデータのストリームは [、MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) 要素と [TimeWindow 要素によって定義](timewindow.md) されます。 [TimeWindow 要素は](timewindow.md)、可用性を照会する期間を定義します。 [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素は [、TimeWindow](timewindow.md)要素からの時刻が **MergedFreeBusy** 要素で返される間隔に分割される方法を定義します。 **MergedFreeBusy** ストリーム内の各数値は [、MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素によって定義される 1 つの間隔を表します。 次の表に、個々の間隔で使用できる値を示します。 
  
|**Digit**|**利用の可否**|
|:-----|:-----|
|0  <br/> |空き  <br/> |
|1  <br/> |仮の予定  <br/> |
|2  <br/> |多忙  <br/> |
|3  <br/> |不在時 (OOF)  <br/> |
|4   <br/> |データなし  <br/> |
   
たとえば、空き時間情報データの要求には、4 時間を表す [TimeWindow](timewindow.md) 要素と、60 分を表す [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) 要素が含まれます。 要求されたユーザーの予定表が最初の 60 分間 OOF で、次の 90 分間ビジー状態で、タイム ウィンドウの最後の 90 分間スケジュールが解除されている場合 **、MergedFreeBusy** ストリームは 3220 になります。 間隔に複数の可用性分類が含まれている場合は、その間隔を分類するために最も高い数値が使用されます。 
  
この要素によって提供される詳細レベルは、要求者に付与されるアクセス許可によって異なります。
  
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

