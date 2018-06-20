---
title: Exchange での EWS の削除に関連するメールボックス イベントのプル通知
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 83511eea-e0b5-4ef0-83b1-0c5434e6d3ab
description: Exchange で EWS を使用してアイテムを削除する場合に、発生するメールボックス イベントを検出します。
ms.openlocfilehash: b12d6a16cc539f36b6b4dcd7274529e9def3c247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759180"
---
# <a name="pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange"></a>Exchange での EWS の削除に関連するメールボックス イベントのプル通知

Exchange で EWS を使用してアイテムを削除する場合に、発生するメールボックス イベントを検出します。
  
トリガー[のアイテムとフォルダーをメールボックスから削除](deleting-items-by-using-ews-in-exchange.md)すると、このメールボックスのイベントです。 異なるバージョンの Exchange は、メールボックスのアイテムとフォルダーに変更への応答として別のメールボックスのイベントを返します。 次の表は、メールボックスのイベントにサブスクライブするのにはプルの通知を使用する場合を削除するために返されるメールボックスのイベントを識別します。 
  
**プル通知用の表 1: メールボックスの削除に関連するイベント**

|**削除し、EWS の操作の種類**|**各フォルダーの識別子を指定すると、Exchange 2010 の通知**|**すべてのフォルダーを指定すると、Exchange 2010 の通知**|**各フォルダーの識別子を指定する場合は、オンラインの Exchange および Exchange 2013 の通知**|**オンラインの Exchange および Exchange 2013 のすべてのフォルダーを指定すると、**|
|:-----|:-----|:-----|:-----|:-----|
|[DeleteItem の操作](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)を使用してソフト削除 <br/> |アイテムに対する DeletedEvent。  <br/> アイテムの親フォルダーの ModifiedEvent です。  <br/> |アイテムに対する DeletedEvent。  <br/> アイテムの親フォルダーの ModifiedEvent です。  <br/> |アイテムに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。アイテムはごみ箱の削除フォルダーに移動されます。  <br/> アイテムの親フォルダーの ModifiedEvent です。  <br/> |アイテムに対する DeletedEvent。  <br/> 既定の検索フォルダー AllItems からのアイテムの DeletedEvent。  <br/> アイテムの親フォルダーの ModifiedEvent です。  <br/> |
|[DeleteItem の操作](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)を使用してハード的に削除します。 <br/> |アイテムに対する DeletedEvent。  <br/> アイテムの親フォルダーの ModifiedEvent です。  <br/> |アイテムに対する DeletedEvent。  <br/> アイテムの親フォルダーの ModifiedEvent です。  <br/> |アイテムに対する DeletedEvent。  <br/> アイテムの親フォルダーの ModifiedEvent です。  <br/> |アイテムに対する DeletedEvent。  <br/> 既定の検索フォルダー AllItems からのアイテムの DeletedEvent。  <br/> アイテムの親フォルダーの ModifiedEvent です。  <br/> |
|[DeleteItem の操作](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)を使用して削除済みアイテム フォルダーに移動します。 <br/> |アイテムに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。  <br/> 項目の古い親フォルダーに ModifiedEvent。  <br/> 項目の新しい親フォルダー、削除済みアイテム フォルダーの ModifiedEvent です。  <br/> |アイテムに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。  <br/> 項目の古い親フォルダーに ModifiedEvent。  <br/> 項目の新しい親フォルダー、削除済みアイテム フォルダーの ModifiedEvent です。  <br/> |アイテムに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。  <br/> 項目の古い親フォルダーに ModifiedEvent。  <br/> 項目の新しい親フォルダー、削除済みアイテム フォルダーの ModifiedEvent です。  <br/> |既定の検索フォルダー AllItems からの DeletedEvent。  <br/> AllItems フォルダーのアイテムに対する CreatedEvent。  <br/> アイテムの元の親フォルダーの ModifiedEvent です。  <br/> 削除済みアイテム フォルダーに対する ModifiedEvent。  <br/> |
|[DeleteFolder 操作](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)を使用してソフト削除 <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに ModifiedEvent。  <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに ModifiedEvent。  <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに ModifiedEvent。  <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに ModifiedEvent。  <br/> |
|[DeleteFolder 操作](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)を使用してハード的に削除します。 <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに ModifiedEvent。  <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに ModifiedEvent。  <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに ModifiedEvent。  <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに ModifiedEvent。  <br/> |
|[DeleteFolder 操作](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)を使用して削除済みアイテム フォルダーに移動します。 <br/> |フォルダーに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。  <br/> フォルダーの古い親フォルダーに ModifiedEvent。  <br/> フォルダーの新しい親フォルダーに、削除済みアイテム フォルダーには ModifiedEvent です。  <br/> |フォルダーに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。  <br/> フォルダーの古い親フォルダーに ModifiedEvent。  <br/> フォルダーの新しい親フォルダーに、削除済みアイテム フォルダーには ModifiedEvent です。  <br/> |フォルダーに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。  <br/> フォルダーの古い親フォルダーに ModifiedEvent。  <br/> フォルダーの新しい親フォルダーに、削除済みアイテム フォルダーには ModifiedEvent です。  <br/> |フォルダーの古い親フォルダーに ModifiedEvent。  <br/> 削除済みアイテム フォルダーであるフォルダーの新しい親フォルダーの ModifiedEvent です。  <br/> |
   
## <a name="see-also"></a>関連項目


- [Notification subscriptions, mailbox events, and EWS in Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Exchange の EWS を使用するアイテムの削除](deleting-items-by-using-ews-in-exchange.md)
    
- [Exchange EWS での削除に関連するエラーの処理](handling-deletion-related-errors-in-ews-in-exchange.md)
    

