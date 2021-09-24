---
title: ReminderIsSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ReminderIsSet
api_type:
- schema
ms.assetid: fa366afe-77a0-4c14-9edb-ffc9699131ba
description: ReminderIsSet 要素は、アラームストア内のアイテムに対してアラームが設定されているかどうかをExchangeします。
ms.openlocfilehash: 2faa32b9b58789ecefd3b0c412d764765d5afada
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513424"
---
# <a name="reminderisset"></a>ReminderIsSet

**ReminderIsSet** 要素は、アラームストア内のアイテムに対してアラームが設定されているかどうかをExchangeします。 
  
```xml
<ReminderIsSet/>
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

テキスト値が **true の場合** は、アラームが設定されています。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

