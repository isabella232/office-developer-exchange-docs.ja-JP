---
title: MergedFreeBusy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusy
api_type:
- schema
ms.assetid: ea45590d-476e-4b68-9fe8-ae392feadfea
description: MergedFreeBusy 要素には、データのマージされた空き時間ストリームが含まれています。
ms.openlocfilehash: a1483449534f0d886e3c97a23d28c5d78f865042
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468727"
---
# <a name="mergedfreebusy"></a>MergedFreeBusy

**MergedFreeBusy**要素には、データのマージされた空き時間ストリームが含まれています。 
  
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
|[FreeBusyView](freebusyview.md) <br/> |特定のユーザーの空き時間情報が保存されています。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>テキスト値

[FreeBusyViewType](freebusyviewtype.md)要素の値が次のいずれかの場合、サーバーによってテキスト値が提供されます。 
  
- DetailedMerged
    
- FreeBusyMerged
    
- MergedOnly
    
テキスト値は、空き時間情報のストリームです。 
  
## <a name="remarks"></a>注釈

この要素によって提供されるデータのストリームは、 [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素および[TimeWindow](timewindow.md)要素によって定義されます。 [TimeWindow](timewindow.md)要素は、可用性を照会した期間を定義します。 [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素は、 [TimeWindow](timewindow.md)要素からの時間を**MergedFreeBusy**要素で返される間隔にどのように分割するかを定義します。 **MergedFreeBusy** stream の各数値は、 [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素によって定義された1つの間隔を表します。 次の表に、個別の間隔に指定できる値を示します。 
  
|**進数**|**可用性**|
|:-----|:-----|
|.0  <br/> |空き  <br/> |
|1   <br/> |仮の予定  <br/> |
|pbm-2  <br/> |多忙  <br/> |
|1/3  <br/> |不在時 (OOF)  <br/> |
|4   <br/> |データなし  <br/> |
   
たとえば、空き時間情報データの要求には、4時間を表す[TimeWindow](timewindow.md)要素と、60分を表す[MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素が含まれています。 要求されたユーザーの予定表が、最初の60分間、次の90分間、およびタイムウィンドウの最終の90分に対して予定外となっている場合、 **MergedFreeBusy**ストリームは3220になります。 間隔に複数の可用性分類が含まれている場合は、その間隔を分類するために最大数が使用されます。 
  
この要素によって提供される詳細レベルは、リクエスターに付与されるアクセス許可によって異なります。
  
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

