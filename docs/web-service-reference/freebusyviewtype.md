---
title: FreeBusyViewType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FreeBusyViewType
api_type:
- schema
ms.assetid: 7c7f82ba-fa52-4a3e-bec7-39d373c66fc7
description: FreeBusyViewType 要素は、応答で返される空き時間情報の種類を表します。
ms.openlocfilehash: 6eec490b39ccb9c02e7a16c8da7cfdd57f9b92c5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509925"
---
# <a name="freebusyviewtype"></a>FreeBusyViewType

**FreeBusyViewType** 要素は、応答で返される空き時間情報の種類を表します。 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[FreeBusyViewType](freebusyviewtype.md)
  
```xml
<FreeBusyViewType>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</FreeBusyViewType>
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
|[FreeBusyView](freebusyview.md) <br/> |特定のユーザーの可用性情報が含まれる。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 次の表に、この要素に使用できる値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |この値は要求に対して無効です。 この値は、応答に対して有効です。  <br/> |
|MergedOnly  <br/> |集計された空き時間情報ストリームを表します。 1 つのフォレスト内のターゲット ユーザーに可用性サービスが構成されていないフォレスト間のシナリオでは、要求者の可用性サービスは、空き時間情報のパブリック フォルダーからターゲット ユーザーの空き時間情報を取得します。 パブリック フォルダーには、結合された形式の空き時間情報だけが格納されるので、使用可能な情報は **MergedOnly** のみです。  <br/> |
|FreeBusy  <br/> |従来の状態情報 (空き時間情報、空き時間情報、暫定的情報、OOF) を表します。 これには、予定の開始/終了時間も含まれます。 このビューは、集計された空き時間情報ストリームの代わりに個々の会議の開始時間と終了時間が提供されるので、従来の空き時間情報ビューよりもリッチです。  <br/> |
|FreeBusyMerged  <br/> |結合された空き時間情報のストリームを使用して **、FreeBusy** のすべてのプロパティを表します。  <br/> |
|詳細  <br/> |従来の状態情報を表します。空き時間情報、空き時間情報、暫定的情報、OOF。予定の開始/終了時間。題、場所、重要度など、予定のさまざまなプロパティを指定します。 この要求されたビューは、要求元のユーザーが特権を持つ情報の最大量を返します。 Microsoft Exchange Server 2003 フォレスト内のユーザーの情報を要求する場合と同様に、マージされた空き時間情報のみを使用できる場合は **、MergedOnly** が返されます。 それ以外の **場合、FreeBusy** **または Detailed** が返されます。  <br/> 配布 **リストに詳細** が指定されている場合、リストのメンバーの空き時間情報がマージされ **、MergedOnly** が返されます。  <br/> |
|Detailedmerged  <br/> |[詳細] のすべてのプロパティ **を、** マージされた空き時間情報のストリームで表します。 たとえば、メールボックスが Exchange 2003 を実行しているコンピューターに存在する場合など、結合された空き時間情報のみを使用できる場合は **、MergedOnly** が返されます。 それ以外の **場合、FreeBusyMerged または** **DetailedMerged が** 返されます。  <br/> |
   
## <a name="remarks"></a>注釈

[FreeBusyView](freebusyview.md)要素を使用する場合は、この要素が必要です。 返される空き時間情報の種類は [、RequestedView 要素で指定](requestedview.md) されます。 この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
次の表は、さまざまなビューの種類と対応する MAPI プロパティに対して返される値を示しています。 各ビューの種類は、以前のビューの種類に基なります。
  
|**FreeBusyViewType**|**Properties**|**MAPI Calendar プロパティ**|
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
|**詳細** <br/> |Out of Office メッセージ (要求された場合)  <br/> ||
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
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

