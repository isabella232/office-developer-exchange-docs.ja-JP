---
title: FreeBusyViewType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyViewType
api_type:
- schema
ms.assetid: 7c7f82ba-fa52-4a3e-bec7-39d373c66fc7
description: FreeBusyViewType 要素は、応答で返される空き時間情報の情報の種類を表します。
ms.openlocfilehash: fe965d062f72d99dff7148f4d00b12fd8c4e1366
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760617"
---
# <a name="freebusyviewtype"></a>FreeBusyViewType

**FreeBusyViewType**要素は、応答で返される空き時間情報の情報の種類を表します。 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[FreeBusyViewType](freebusyviewtype.md)
  
```xml
<FreeBusyViewType>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</FreeBusyViewType>
```

 **FreeBusyViewType**
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

テキスト値は必須です。 次の表は、この要素の有効な値を一覧します。
  
|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |この値は、要求に対して有効ではありません。 この値は応答をします。  <br/> |
|MergedOnly  <br/> |集計の空き/予約済みのストリームを表します。 1 つのフォレスト内の移動先のユーザーが、可用性サービスが構成されているフォレスト間のシナリオでは、要求側の可用性サービスは、空き時間情報パブリック フォルダーからターゲット ユーザーの空き時間情報を取得します。 パブリック フォルダーは、差し込み印刷の形式でのみ空き時間情報を格納するため**MergedOnly**はのみ利用可能な情報です。  <br/> |
|空き時間情報  <br/> |従来のステータス情報を表します。 フリー、予定あり、仮の予定、および不在時。 これには、予定の開始/終了時刻も含まれています。 このビューは、豊富な集計の空き時間情報のストリームではなく、時間が用意されている個々 の会議の開始し、終了のために表示、レガシ空き時間情報よりも。  <br/> |
|FreeBusyMerged  <br/> |結合された空き時間情報の可用性情報のストリームを**空き時間情報**のすべてのプロパティを表します。  <br/> |
|Detailed  <br/> |従来のステータス情報を表します: 無料、ビジー状態で、仮の予定と OOF。予定の開始/終了時刻予定の件名、場所、および重要度などのさまざまなプロパティを選択します。 この要求されたビューでは、要求元のユーザーの特権の情報量の最大を返します。 結合された空き時間情報のみがある場合と、Microsoft Exchange Server 2003 フォレスト内のユーザーの情報を要求すると**MergedOnly**が返されます。 それ以外の場合、**空き時間情報**や**詳細**が返されます。  <br/> 配布リストの**詳細**を指定すると、そのリストのメンバーの空き時間情報が差し込まれると、 **MergedOnly**が返されます。  <br/> |
|DetailedMerged  <br/> |ストリームの結合された空き時間情報の可用性情報の**詳細**のすべてのプロパティを表します。 結合された空き時間情報がある、たとえば、メールボックスが Exchange 2003 を実行するコンピューター上に存在する場合、だけの場合は、 **MergedOnly**が返されます。 それ以外の場合、 **FreeBusyMerged**または**DetailedMerged**が返されます。  <br/> |
   
## <a name="remarks"></a>備考

[FreeBusyView](freebusyview.md)要素を使用する場合、この要素が必要です。 返される空き時間情報の種類は、 [RequestedView](requestedview.md)要素で指定されます。 MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。 
  
次の表は、別のビューの種類と対応する MAPI プロパティに対して返されるを示します。 各ビューの種類は、以前のビューの種類に基づいて構築します。
  
|**FreeBusyViewType**|**新しいプロパティ**|**MAPI 予定表のプロパティ**|
|:-----|:-----|:-----|
|**MergedOnly** <br/> |MergedFreeBusyStream  <br/> ||
|**空き時間情報** <br/> |古典の状態  <br/> |PropTag (0x80860003)  <br/> |
|**空き時間情報** <br/> |作業時間  <br/> ||
|**空き時間情報** <br/> |開始時刻  <br/> |単に PR_START_DATE  <br/> |
|**空き時間情報** <br/> |終了時刻  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |古典の状態  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusyMerged** <br/> |作業時間  <br/> ||
|**FreeBusyMerged** <br/> |開始時刻  <br/> |単に PR_START_DATE  <br/> |
|**FreeBusyMerged** <br/> |終了時刻  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**詳細** <br/> |古典の状態  <br/> |PropTag (0x80860003)  <br/> |
|**詳細** <br/> |作業時間  <br/> ||
|**詳細** <br/> |開始時刻  <br/> |単に PR_START_DATE  <br/> |
|**詳細** <br/> |終了時刻  <br/> |PR_END_DATE  <br/> |
|**詳細** <br/> |件名  <br/> |あるの PR_SUBJECT  <br/> |
|**詳細** <br/> |場所  <br/> |PR_LOCATION  <br/> |
|**詳細** <br/> |エントリ Id(unless private)  <br/> ||
|**詳細** <br/> |プライベート フラグ  <br/> ||
|**詳細** <br/> |IsMeeting  <br/> ||
|**詳細** <br/> |IsRecurring  <br/> ||
|**詳細** <br/> |IsException  <br/> ||
|**詳細** <br/> |IsReminderSet  <br/> ||
|**詳細** <br/> |Office のメッセージ (要求された場合)  <br/> ||
|**DetailedMerged** <br/> |古典の状態  <br/> |PropTag (0x80860003)  <br/> |
|**DetailedMerged** <br/> |作業時間  <br/> ||
|**DetailedMerged** <br/> |開始時刻  <br/> |単に PR_START_DATE  <br/> |
|**DetailedMerged** <br/> |終了時刻  <br/> |PR_END_DATE  <br/> |
|**DetailedMerged** <br/> |件名  <br/> |あるの PR_SUBJECT  <br/> |
|**DetailedMerged** <br/> |場所  <br/> |PR_LOCATION  <br/> |
|**DetailedMerged** <br/> |エントリ Id(unless private)  <br/> ||
|**DetailedMerged** <br/> |プライベート フラグ  <br/> ||
|**DetailedMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**DetailedMerged** <br/> |IsMeeting  <br/> ||
|**DetailedMerged** <br/> |IsRecurring  <br/> ||
|**DetailedMerged** <br/> |IsException  <br/> ||
|**DetailedMerged** <br/> |IsReminderSet  <br/> ||
   
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

