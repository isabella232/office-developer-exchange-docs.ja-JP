---
title: HasAttachments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasAttachments
api_type:
- schema
ms.assetid: 538b7a85-11d7-4daa-8458-09b540760e8b
description: HasAttachments 要素は、アイテムに少なくとも1つの添付ファイルがある場合、または添付ファイルを持つアイテムが1つ以上含まれている場合に、true に設定されるプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。
ms.openlocfilehash: cc4e4ec0eac1c749723facc8cd780da41b0d8150
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462923"
---
# <a name="hasattachments"></a>HasAttachments

**Hasattachments**要素は、アイテムに少なくとも1つの添付ファイルがある場合、または添付ファイルを持つアイテムが1つ以上含まれている場合に、 **true**に設定されるプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 
  
```XML
<HasAttachments/>
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
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[条件](conditions.md) <br/> |そのルールのルールの処理を開始するときに実行される条件を表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[会話 (ConversationType)](conversation-conversationtype.md) <br/> |単一の会話を表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[例外](exceptions.md) <br/> |受信トレイルールの利用可能なすべてのルールの例外条件を表します。  <br/> |
|[Item](item.md) <br/> |Exchange ストア内のアイテムを表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メールメッセージを表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値を表すテキスト値が必要です。 値が**true**の場合は、アイテムまたはスレッドに表示されている添付ファイルが1つ以上あることを意味します。 値が**false**の場合は、アイテムまたは会話に添付ファイルがないか、または添付ファイルのみが含まれていることを意味します。 
  
## <a name="remarks"></a>注釈

**Hasattachments**プロパティは、ブール値の**AllAttachmentsHidden** MAPI プロパティから計算されます。 アイテムに添付ファイルがない場合、 **AllAttachmentsHidden**プロパティは存在しません。 アイテムのすべての添付ファイルが非表示になっている場合、 **AllAttachmentsHidden**プロパティは**true**になります。 少なくとも1つの添付ファイルがあり、少なくとも1つの添付ファイルが表示されている場合、 **AllAttachmentsHidden**プロパティは**false**になります。 **AllAttachmentsHidden** MAPI プロパティを使用して、アイテムの検索、グループ化、および並べ替えを行います。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
  
[Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)

