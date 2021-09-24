---
title: RequestedView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RequestedView
api_type:
- schema
ms.assetid: e2b4cf8c-5d43-4cd8-b86d-cc27a5d2f095
description: RequestView 要素は、クライアントが要求する予定表情報の種類を定義します。
ms.openlocfilehash: 350922a7fef90c26ace0ef8be07ebb866d304eb3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509477"
---
# <a name="requestedview"></a>RequestedView

**RequestView 要素** は、クライアントが要求する予定表情報の種類を定義します。 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[RequestedView](requestedview.md)
  
```xml
<RequestedView>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</RequestedView>
```

 **FreeBusyViewType**
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

テキスト値は必須です。 次の表に、この要素に使用できる値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |この値は要求に対して無効です。 この値は、応答に対して有効です。  <br/> |
|MergedOnly  <br/> |集計された空き時間情報ストリームを表します。 1 つのフォレスト内のターゲット ユーザーに可用性サービスが構成されていないフォレスト間のシナリオでは、要求者の可用性サービスは、空き時間情報のパブリック フォルダーからターゲット ユーザーの空き時間情報を取得します。 パブリック フォルダーには、結合された形式の空き時間情報だけが格納されるので、使用可能な情報は **MergedOnly** のみです。  <br/> |
|FreeBusy  <br/> |従来の状態情報 (空き時間情報、空き時間情報、暫定的情報、OOF) を表します。 これには、予定の開始/終了時間も含まれます。 このビューは、集計された空き時間情報ストリームの代わりに個々の会議の開始時間と終了時間が提供されるので、従来の空き時間情報ビューよりもリッチです。  <br/> |
|FreeBusyMerged  <br/> |結合された空き時間情報の **ストリームで FreeBusy** のすべてのプロパティを表します。  <br/> |
|詳細  <br/> |従来の状態情報を表します。空き時間情報、空き時間情報、暫定的情報、OOF。予定の開始/終了時間。題、場所、重要度など、予定のさまざまなプロパティを指定します。 この要求されたビューは、要求元のユーザーが特権を持つ情報の最大量を返します。 Microsoft Exchange Server 2003 フォレスト内のユーザーの情報を要求する場合と同様に、マージされた空き時間情報のみを使用できる場合は **、MergedOnly** が返されます。 それ以外の **場合、FreeBusy** **または Detailed** が返されます。  <br/> |
|Detailedmerged  <br/> |[詳細] のすべてのプロパティ **を、結合** された空き時間情報のストリームで表します。 マージされた空き時間情報のみを使用できる場合は **、MergedOnly が** 返されます。 それ以外の **場合、FreeBusyMerged または** **DetailedMerged が** 返されます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素によって設定された値は、応答で [FreeBusyViewType](freebusyviewtype.md) 要素と一緒に返されます。 
  
次の表は、さまざまなビューの種類と対応する MAPI プロパティに対して返される値を示しています。 各ビューの種類は、以前のビューの種類に基なります。
  
|**空き時間情報ビューの種類**|**Properties**|**MAPI Calendar プロパティ**|
|:-----|:-----|:-----|
|**MergedOnly** <br/> |MergedFreeBusyStream  <br/> ||
|**FreeBusy** <br/> |従来の状態  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusy** <br/> |就業時間  <br/> ||
|**FreeBusy** <br/> |開始時刻  <br/> |PR_START_DATE  <br/> |
|**FreeBusy** <br/> |終了時刻  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |従来の状態  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusyMerged** <br/> |就業時間  <br/> ||
|**FreeBusyMerged** <br/> |開始時刻  <br/> |PR_START_DATE  <br/> |
|**FreeBusyMerged** <br/> |終了時刻  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**詳細** <br/> |従来の状態  <br/> |PropTag (0x80860003)  <br/> |
|**詳細** <br/> |就業時間  <br/> ||
|**詳細** <br/> |開始時刻  <br/> |PR_START_DATE  <br/> |
|**詳細** <br/> |終了時刻  <br/> |PR_END_DATE  <br/> |
|**詳細** <br/> |件名  <br/> |PR_SUBJECT  <br/> |
|**詳細** <br/> |Location  <br/> |PR_LOCATION  <br/> |
|**詳細** <br/> |Entry-Id(private を指定しない場合)  <br/> ||
|**詳細** <br/> |プライベート フラグ  <br/> ||
|**詳細** <br/> |IsMeeting  <br/> ||
|**詳細** <br/> |IsRecurring  <br/> ||
|**詳細** <br/> |IsException  <br/> ||
|**詳細** <br/> |IsReminderSet  <br/> ||
|**Detailedmerged** <br/> |従来の状態  <br/> |PropTag (0x80860003)  <br/> |
|**Detailedmerged** <br/> |就業時間  <br/> ||
|**Detailedmerged** <br/> |開始時刻  <br/> |PR_START_DATE  <br/> |
|**Detailedmerged** <br/> |終了時刻  <br/> |PR_END_DATE  <br/> |
|**Detailedmerged** <br/> |件名  <br/> |PR_SUBJECT  <br/> |
|**Detailedmerged** <br/> |Location  <br/> |PR_LOCATION  <br/> |
|**Detailedmerged** <br/> |Entry-Id(private を指定しない場合)  <br/> ||
|**Detailedmerged** <br/> |プライベート フラグ  <br/> ||
|**Detailedmerged** <br/> |MergedFreeBusyStream  <br/> ||
|**Detailedmerged** <br/> |IsMeeting  <br/> ||
|**Detailedmerged** <br/> |IsRecurring  <br/> ||
|**Detailedmerged** <br/> |IsException  <br/> ||
|**Detailedmerged** <br/> |IsReminderSet  <br/> ||
   
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

