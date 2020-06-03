---
title: DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 055cdee8-3c7d-47db-9f27-740f4a674729
description: DeleteItem 要素は、Exchange ストア内のメールボックスからアイテムを削除するための要求を定義します。
ms.openlocfilehash: ed13ee32b487f49740aed80e8705257d3e2e6938
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529204"
---
# <a name="deleteitem"></a>DeleteItem

**DeleteItem**要素は、Exchange ストア内のメールボックスからアイテムを削除するための要求を定義します。 
  
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
|**DeleteType** <br/> |アイテムが削除される方法について説明します。 この属性は必須です。  <br/> |
|**Send会議のキャンセル** <br/> |予定表アイテムの削除が出席者に伝達されるかどうかを指定します。 この属性は、予定表アイテムが削除されるときに必要になります。 非予定表アイテムが削除された場合、この属性は省略可能です。  <br/> |
|**AffectedTaskOccurrences** <br/> |[DeleteItem 操作](deleteitem-operation.md)によってタスクインスタンスまたはタスクマスターが削除されるかどうかを指定します。 この属性は、タスクを削除するときに必要になります。 非タスクアイテムが削除されている場合、この属性は省略可能です。  <br/> |
|**SuppressReadReceipts** <br/> |削除済みアイテムの開封確認を抑制するかどうかを示します。 テキスト値が**true**の場合、開封確認が抑制されることを示します。 値が**false**の場合、開封確認が送信者に送信されることを示します。 この属性は省略可能です。  <br/> |
   
#### <a name="deletetype-attribute"></a>DeleteType 属性

|**値**|**説明**|
|:-----|:-----|
|HardDelete  <br/> |アイテムがストアから完全に削除されます。  <br/> |
|SoftDelete  <br/> |収集が有効になっている場合、アイテムは収集に移動されます。  <br/> |
|MoveToDeletedItems  <br/> |アイテムが [削除済みアイテム] フォルダーに移動されます。  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a>Send会議のキャンセル属性

|**値**|**説明**|
|:-----|:-----|
|SendToNone  <br/> |キャンセルメッセージを送信せずに予定表アイテムが削除されます。  <br/> |
|SendOnlyToAll  <br/> |予定表アイテムが削除され、すべての出席者に取り消しメッセージが送信されます。  <br/> |
|SendToAllAndSaveCopy  <br/> |予定表アイテムが削除され、すべての出席者に取り消しメッセージが送信されます。 取り消しメッセージのコピーが [送信済みアイテム] フォルダーに保存されます。  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a>AffectedTaskOccurrences 属性

|**値**|**説明**|
|:-----|:-----|
|AllOccurrences  <br/> |アイテムの削除要求は、マスタータスクを削除します。したがって、マスタータスクに関連付けられているすべての定期的なタスクを削除します。  <br/> |
|変数のみ  <br/> |アイテムの削除要求では、タスクの特定のオカレンスのみが削除されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Exchange ストア内のメールボックスから削除する項目、オカレンスアイテム、定期的なマスターアイテムの配列を格納します。 [DeleteItem 操作](deleteitem-operation.md)は、任意のアイテムの種類に対して実行できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

**MoveToDeletedItems**および**ハード削除**オプションは、トランザクションであり、Web サービスの呼び出しが完了すると、データベースがアイテムを削除済みアイテムフォルダーに移動したか、または Exchange データベースからアイテムを完全に削除したことを意味します。 この動作は、Microsoft Exchange Server 2007 および Exchange Server 2010 の場合と同じです。 
  
**Softdelete**オプションは、Exchange のターゲットバージョンによって動作が異なります。 Exchange 2007 用の**Softdelete**は、今後、不確定な時点でアイテムが収集フォルダーに移動されることを exchange データベースに示すように、アイテムのビットを設定します。 Exchange 2010 用の**Softdelete**は、直ちにアイテムを収集に移動します。 **Softdelete**はフォルダー削除のオプションではありません。 **ソフト削除**によるアイテムとフォルダーの検索では、結果は返されません。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [DeleteItemResponse](deleteitemresponse.md)  
- [DeleteItem 操作](deleteitem-operation.md)

