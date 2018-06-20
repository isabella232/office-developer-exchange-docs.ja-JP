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
description: 添付ファイル付きの要素は、項目が、表示されている 1 つ以上の添付ファイルまたは添付ファイルのある場合は、テーマには、少なくとも 1 つの項目が含まれている場合、true に設定されているプロパティを表します。 このプロパティは値の取得のみ可能です。
ms.openlocfilehash: e76e0ecbb357396540f0d1649cf5062edfb18660
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831801"
---
# <a name="hasattachments"></a>HasAttachments

**添付ファイル付き**の要素は、項目が、表示されている 1 つ以上の添付ファイルまたは添付ファイルのある会話には、少なくとも 1 つの項目が含まれている場合に**true**に設定されているプロパティを表します。 このプロパティは値の取得のみ可能です。 
  
```XML
<HasAttachments/>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[条件](conditions.md) <br/> |条件を表しますが、満たされるとときに、そのルールのルールの処理をトリガーします。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[会話 (ConversationType)](conversation-conversationtype.md) <br/> |1 つのテーマを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[Exceptions](exceptions.md) <br/> |受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。  <br/> |
|[アイテム](item.md) <br/> |Exchange ストア内の項目を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消し通知を表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の返信を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メール メッセージを表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値を表す文字列値は、必要があります。 **True**の場合は、会話または複数のアイテムが表示されている 1 つ以上の添付ファイルを持っているを意味します。 **False**の値は、アイテムまたは会話ことか、添付ファイルがないか、添付ファイルを非表示にのみを意味します。 
  
## <a name="remarks"></a>備考

**添付ファイル付き**のプロパティは、ブール値の**AllAttachmentsHidden**の MAPI プロパティから計算されます。 アイテムが添付ファイルを持たない場合、 **AllAttachmentsHidden**プロパティは存在しません。 アイテムのすべての添付ファイルが表示されない場合は、 **AllAttachmentsHidden**プロパティが**true**です。 1 つ以上の添付ファイルがあり、1 つ以上の添付ファイルが表示されている場合、 **AllAttachmentsHidden**プロパティは**false**です。 **AllAttachmentsHidden** MAPI プロパティを使用して、検索、グループ化、およびアイテムの並べ替えをします。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
  

  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)

