---
title: サイズ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Size
api_type:
- schema
ms.assetid: 966f4daf-c20e-49f8-aeb6-965f3e2da7c3
description: サイズの要素は、現在のフォルダー内の会話ですべてのアイテムのバイト単位のサイズを表します。 このプロパティは値の取得のみ可能です。
ms.openlocfilehash: 15ee0bce6bc5fa2065cef4ecee40d7a6d65e3249
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833509"
---
# <a name="size"></a>サイズ

**サイズ**の要素は、現在のフォルダー内の会話ですべてのアイテムのバイト単位のサイズを表します。 このプロパティは値の取得のみ可能です。 
  
```XML
<Size/>
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
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[会話 (ConversationType)](conversation-conversationtype.md) <br/> |1 つのテーマを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Exchange ストア内のアイテムに関連付けられているファイルを表します。  <br/> |
|[アイテム](item.md) <br/> |Exchange ストア内の項目を表します。  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消し通知を表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の返信を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メール メッセージを表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |Exchange ストアから項目を削除します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、バイト内の項目のサイズを識別する整数値です。
  
## <a name="remarks"></a>備考

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

