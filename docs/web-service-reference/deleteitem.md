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
description: DeleteItem 要素は、Exchange ストア内のメールボックスからアイテムを削除する要求を定義します。
ms.openlocfilehash: de64787750c88c8a47bb69daddc0a1d2ebe8bde9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759990"
---
# <a name="deleteitem"></a>DeleteItem

**DeleteItem**要素は、Exchange ストア内のメールボックスからアイテムを削除する要求を定義します。 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 **DeleteItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**削除の種類** <br/> |アイテムを削除する方法について説明します。 この属性は、必要があります。  <br/> |
|**SendMeetingCancellations** <br/> |予定表アイテムの削除を参加者に伝達するかどうかについて説明します。 予定表アイテムが削除されたとき、この属性が必要です。 この属性は、非予定表アイテムが削除された場合は省略可能です。  <br/> |
|**AffectedTaskOccurrences** <br/> |[DeleteItem 操作](deleteitem-operation.md)によって、タスクのインスタンスまたはタスク マスターを削除するかどうかについて説明します。 タスクが削除されるとき、この属性が必要です。 以外の項目が削除されたとき、この属性はオプションです。  <br/> |
|**SuppressReadReceipts** <br/> |削除済みアイテムの開封確認メッセージを抑制するかどうかを示します。 テキストの値**は true**では、開封確認のメッセージが抑制されていることを示します。 **False**の値は、送信者に開封確認を送信することを示します。 この属性は、省略可能です。  <br/> |
   
#### <a name="deletetype-attribute"></a>削除の種類の属性

|**値**|**説明**|
|:-----|:-----|
|HardDelete  <br/> |アイテムはストアから完全に削除されます。  <br/> |
|SoftDelete  <br/> |アイテムを移動、ごみ箱をあさる場合、収集を有効にします。  <br/> |
|MoveToDeletedItems  <br/> |アイテムは、削除済みアイテム フォルダーに移動されます。  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a>SendMeetingCancellations 属性

|**値**|**説明**|
|:-----|:-----|
|SendToNone  <br/> |取り消しメッセージを送信することがなく、予定表アイテムが削除されます。  <br/> |
|SendOnlyToAll  <br/> |予定表アイテムが削除され、すべての出席者にキャンセル通知が送信されます。  <br/> |
|SendToAllAndSaveCopy  <br/> |予定表アイテムが削除され、すべての出席者にキャンセル通知が送信されます。 取り消しについてのメッセージのコピーは、送信済みアイテム フォルダーに保存されます。  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a>AffectedTaskOccurrences 属性

|**値**|**説明**|
|:-----|:-----|
|AllOccurrences  <br/> |削除項目の要求は、マスターのタスクを削除し、したがってすべての定期的なタスクに関連付けられているマスターのタスクします。  <br/> |
|SpecifiedOccurrenceOnly  <br/> |削除項目の要求では、タスクの特定の個所だけを削除します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Itemid](itemids.md) <br/> |アイテム、出現アイテム、および Exchange ストアのメールボックスから削除するのにはマスターの定期的なアイテムの配列が含まれています。 [DeleteItem の操作](deleteitem-operation.md)は、任意の項目の種類を実行できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

**MoveToDeletedItems**および**HardDelete**オプションは、時間によって、Web サービスの呼び出しが完了していることを意味する、トランザクション、データベースは削除済みアイテム フォルダーにアイテムを移動または Exchange データベースから項目を完全に削除します。 この現象は、MicrosoftExchange Server 2007 および Exchange Server 2010 と同じです。 
  
**SoftDelete**オプションの動作は別のターゲットのバージョンの Exchange で異なります。 Exchange 2007 用の**SoftDelete**のビット設定項目を示す項目を移動する Exchange データベースに、ごみ箱をあさる時に、不確定な将来のフォルダーです。 Exchange 2010 の**SoftDelete**はすぐにアイテムを移動、ごみ箱をあさる。 **SoftDelete**は、フォルダーの削除のオプションではありません。 アイテムとフォルダーの**SoftDelete**の走査の検索では、結果は返されません。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [DeleteItemResponse](deleteitemresponse.md)  
- [DeleteItem の操作](deleteitem-operation.md)

