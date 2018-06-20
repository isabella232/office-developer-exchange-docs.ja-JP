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
description: MergedFreeBusy 要素には、マージされた空き時間情報データ ストリームが含まれています。
ms.openlocfilehash: 542b9fae0c36b0236bd806e8a9117753968e812c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832449"
---
# <a name="mergedfreebusy"></a>MergedFreeBusy

**MergedFreeBusy**要素には、マージされた空き時間情報データ ストリームが含まれています。 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[MergedFreeBusy](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FreeBusyView](freebusyview.md) <br/> |特定のユーザーの利用可能時間情報が含まれています。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、 [FreeBusyViewType](freebusyviewtype.md)要素の値は、次のいずれかの場合、サーバーにより提供されます。 
  
- DetailedMerged
    
- FreeBusyMerged
    
- MergedOnly
    
テキスト値は、空き時間情報のストリームです。 
  
## <a name="remarks"></a>備考

この要素によって提供されるデータのストリームは、 [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)と[時間](timewindow.md)の要素によって定義されます。 [時間](timewindow.md)要素では、可用性のクエリを実行する時間間隔を定義します。 [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素は、 **MergedFreeBusy**要素で返される間隔に[時間](timewindow.md)の要素からの時間を分割する方法を定義します。 **MergedFreeBusy**ストリームのそれぞれの数値は、 [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素で定義されている 1 つの間隔を表します。 次の表は、個々 の間隔の可能な値を一覧します。 
  
|**桁**|**可用性**|
|:-----|:-----|
|0  <br/> |Free  <br/> |
|1  <br/> |Tentative  <br/> |
|2  <br/> |Busy  <br/> |
|3  <br/> |不在時 (OOF)  <br/> |
|4  <br/> |データがありません。  <br/> |
   
たとえば、空き時間情報データに対する要求には、4 つの時間を表す[時間](timewindow.md)の要素と 60 分を表す[MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素が含まれています。 要求されたユーザーの予定表では、不在時の最初の 60 分間、次の 90 分の時間と時間ウィンドウで、最後の 90 分間予定されていない**MergedFreeBusy**ストリームなります 3220。 間隔には、2 つ以上の可用性のクラス分けが含まれています、その間隔を分類する最上位の番号が使用されます。 
  
この要素によって提供される詳細のレベルは、要求側に付与するアクセス許可に依存します。
  
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

