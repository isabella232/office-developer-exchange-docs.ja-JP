---
title: TimeWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeWindow
api_type:
- schema
ms.assetid: 49c79266-353a-4036-a8e2-8a4660d0d8ea
description: TimeWindow 要素は、ユーザーの可用性情報に対してクエリを実行した期間を識別します。
ms.openlocfilehash: 93a486a5bc2306cfa61b74de82d795a711dbbceb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531345"
---
# <a name="timewindow"></a>TimeWindow

**TimeWindow 要素は**、ユーザーの可用性情報に対してクエリを実行した期間を識別します。 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[TimeWindow](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 **Duration**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |ユーザーの可用性情報に対してクエリを実行した期間の開始を表します。  <br/> |
|[EndTime](endtime.md) <br/> |ユーザーの可用性情報に対してクエリを実行した期間の終了を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |応答で返される空き時間情報の種類を指定します。  <br/> 次に、この要素の XPath を示します。  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a>注釈

この期間の最大値は 42 日です。 この最大値は変更できます。 最大値を超えるユーザー可用性情報の要求はエラーを返します。 StartTime 要素と[EndTime](starttime.md)要素によって定義された期間に予定が[](endtime.md)部分的に含まれている場合、その予定は全体に含まれます。 
  
> [!NOTE]
> この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft® Exchange Server 2007 を実行しているコンピューターの /EWS/ ディレクトリにあります。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)


[ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

