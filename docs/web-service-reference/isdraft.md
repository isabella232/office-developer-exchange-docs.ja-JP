---
title: IsDraft
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsDraft
api_type:
- schema
ms.assetid: 8b8d9cc9-a512-458a-94e4-af210ac83bd7
description: IsDraft 要素は、アイテムがまだ送信されていないかどうかを示します。
ms.openlocfilehash: 20acbbdd1148208f6cd9160f2f3879617663ab0a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512877"
---
# <a name="isdraft"></a>IsDraft

**IsDraft 要素** は、アイテムがまだ送信されていないかどうかを示します。 
  
```xml
<IsDraft/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[Contact](contact.md) <br/> |連絡先アイテムExchangeを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[項目](item.md) <br/> |ストア内のアイテムをExchangeします。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |会議ストアでの会議の取り消しExchangeします。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |ユーザー ストア内の会議Exchangeします。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |会議ストアの会議の応答Exchangeします。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |電子メール メッセージExchangeを表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |アイテムをストアからExchangeします。  <br/> |
|[タスク](task.md) <br/> |ストア内のタスクをExchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値を表すテキスト値が必要です。 値 true は **、** メッセージがまだ送信されていない状態を示します。 false の **値は** 、メッセージが送信されたかどうかを示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

