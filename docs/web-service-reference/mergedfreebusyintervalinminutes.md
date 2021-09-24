---
title: MergedFreeBusyIntervalInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MergedFreeBusyIntervalInMinutes
api_type:
- schema
ms.assetid: 481cdbc6-d5aa-49fa-a3fa-9d119d3dca99
description: MergedFreeBusyIntervalInMinutes 要素は、FreeBusyMerged ビューの連続する 2 つのスロット間の時間差を表します。
ms.openlocfilehash: 543a631ffe85e50e3efe84fb8109b190a276ed8f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532391"
---
# <a name="mergedfreebusyintervalinminutes"></a>MergedFreeBusyIntervalInMinutes

**MergedFreeBusyIntervalInMinutes** 要素は **、FreeBusyMerged** ビューの連続する 2 つのスロット間の時間差を表します。 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)
  
```xml
<MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
```

 **int**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |応答で返される空き時間情報の種類を指定します。  <br/> 次に、この要素の XPath を示します。  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は時間 (分) を表します。 既定値は 30 分です。 6 分は最小間隔で、1 日 (1440 分) は、この要素の最大間隔です。
  
## <a name="remarks"></a>注釈

この値は [、RequestedView](requestedview.md)要素が **MergedOnly、FreeBusyMerged、** または **DetailedMerge** に等しい場合にのみ使用されます。  これは整数データ型です。 この要素によって定義された間隔を含むストリームは [、MergedFreeBusy 要素に返](mergedfreebusy.md) されます。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserOofSettings 操作](getuseroofsettings-operation.md)


[ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

