---
title: DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 055cdee8-3c7d-47db-9f27-740f4a674729
description: DeleteItem 要素は、アイテム ストア内のメールボックスからアイテムを削除する要求Exchangeします。
ms.openlocfilehash: aa421de447126a22c1f01b3a0dc7498ff5b74a65
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528888"
---
# <a name="deleteitem"></a>DeleteItem

**DeleteItem 要素** は、メールボックス ストア内のメールボックスからアイテムを削除する要求Exchangeします。 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 **DeleteItemType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**DeleteType** <br/> |アイテムを削除する方法について説明します。 この属性は必須です。  <br/> |
|**SendMeetingCancellations** <br/> |予定表アイテムの削除が出席者に伝達されるかどうかを示します。 この属性は、予定表アイテムが削除される場合に必要です。 予定表以外のアイテムが削除される場合、この属性はオプションです。  <br/> |
|**AffectedTaskOccurrences** <br/> |タスク インスタンスまたはタスク マスターが DeleteItem 操作によって削除されるかどうかを [示します](deleteitem-operation.md)。 この属性は、タスクが削除される場合に必要です。 タスク以外のアイテムが削除される場合、この属性はオプションです。  <br/> |
|**SuppressReadReceipts** <br/> |削除されたアイテムの読み取りレシートを非表示にするかどうかを示します。 テキスト値が **true の** 場合は、読み取りレシートが表示されません。 値 false **は、** 読み取りレシートが送信者に送信されるかどうかを示します。 この属性は省略可能です。  <br/> |
   
#### <a name="deletetype-attribute"></a>DeleteType 属性

|**値**|**説明**|
|:-----|:-----|
|HardDelete  <br/> |アイテムはストアから完全に削除されます。  <br/> |
|SoftDelete  <br/> |ダンプスターが有効になっている場合、アイテムはゴミ箱に移動されます。  <br/> |
|MoveToDeletedItems  <br/> |アイテムが [削除済みアイテム] フォルダーに移動されます。  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a>SendMeetingCancellations 属性

|**値**|**説明**|
|:-----|:-----|
|SendToNone  <br/> |キャンセル メッセージを送信せずに予定表アイテムが削除されます。  <br/> |
|SendOnlyToAll  <br/> |予定表アイテムが削除され、キャンセル メッセージがすべての出席者に送信されます。  <br/> |
|SendToAllAndSaveCopy  <br/> |予定表アイテムが削除され、キャンセル メッセージがすべての出席者に送信されます。 キャンセル メッセージのコピーが [送信済みアイテム] フォルダーに保存されます。  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a>AffectedTaskOccurrences 属性

|**値**|**説明**|
|:-----|:-----|
|AllOccurrences  <br/> |アイテムの削除要求では、マスター タスクが削除されるため、マスター タスクに関連付けられているすべての定期的なタスクが削除されます。  <br/> |
|SpecifiedOccurrenceOnly  <br/> |削除アイテム要求は、タスクの特定の出現回数のみを削除します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |アイテム、オカレンス アイテム、および定期的なマスター アイテムの配列を含み、アイテム ストア内のメールボックスからExchangeします。 [DeleteItem 操作は、](deleteitem-operation.md)任意の種類のアイテムに対して実行できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

**MoveToDeletedItems** および **HardDelete** オプションはトランザクションであり、Web サービス呼び出しが完了すると、データベースはアイテムを削除済みアイテム フォルダーに移動するか、Exchange データベースからアイテムを完全に削除しました。 この動作は、MicrosoftExchange Server 2007 および 2010 Exchange Serverです。 
  
**SoftDelete オプションは**、ターゲット バージョンごとに異なる方法で動作Exchange。 Exchange 2007 の **SoftDelete** は、アイテムが将来不確定な時期にゴミ箱フォルダーに移動することを Exchange データベースに示すアイテムに少し設定します。 **SoftDelete** for Exchange 2010 は、アイテムをすぐにゴミ箱に移動します。 **SoftDelete** はフォルダー削除のオプションではありません。 **アイテムとフォルダーの SoftDelete** traversal 検索では、結果は返されません。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [DeleteItemResponse](deleteitemresponse.md)  
- [DeleteItem 操作](deleteitem-operation.md)

