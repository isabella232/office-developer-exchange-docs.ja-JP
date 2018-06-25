---
title: MergedFreeBusyIntervalInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusyIntervalInMinutes
api_type:
- schema
ms.assetid: 481cdbc6-d5aa-49fa-a3fa-9d119d3dca99
description: MergedFreeBusyIntervalInMinutes 要素は、FreeBusyMerged のビューで連続する 2 つのスロット間の時間差を表します。
ms.openlocfilehash: 99c8c69424a0a9d9594005fdf6b2ceba53e6288a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832451"
---
# <a name="mergedfreebusyintervalinminutes"></a>MergedFreeBusyIntervalInMinutes

**MergedFreeBusyIntervalInMinutes**要素は、 **FreeBusyMerged**のビューで連続する 2 つのスロット間の時間差を表します。 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)
  
```xml
<MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
```

 **int**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |応答で返される空き時間情報の情報の種類を指定します。  <br/> 以下は、この要素の XPath です。  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、分単位の時間を表します。 既定値は、30 分です。 6 分間隔の最小値は、1 日 (1440 分) この要素の最大間隔。
  
## <a name="remarks"></a>備考

[RequestedView](requestedview.md)要素は、 **MergedOnly**、 **FreeBusyMerged**、または**DetailedMerge**に等しい場合にのみ、この値が使用されます。 これは、整数データ型です。 [MergedFreeBusy](mergedfreebusy.md)要素では、この要素で定義された間隔を格納しているストリームが返されます。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserOofSettings 操作](getuseroofsettings-operation.md)


[ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

