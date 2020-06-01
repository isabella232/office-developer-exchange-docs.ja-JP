---
title: Exchange での EWS の削除に関連するメールボックス イベントのプル通知
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 83511eea-e0b5-4ef0-83b1-0c5434e6d3ab
description: Exchange で EWS を使用してアイテムを削除する場合に、発生するメールボックス イベントを検出します。
ms.openlocfilehash: c3d98ff798e3d0f6d214111d51da2c81278fd17d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457656"
---
# <a name="pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange"></a>Exchange での EWS の削除に関連するメールボックス イベントのプル通知

Exchange で EWS を使用してアイテムを削除する場合に、発生するメールボックス イベントを検出します。
  
[アイテムとフォルダーをメールボックスから削除する](deleting-items-by-using-ews-in-exchange.md)と、メールボックスのイベントがトリガーされます。バージョンが異なる Exchange では、メールボックスのアイテムとフォルダーの変更に対する応答として別のメールボックス イベントを返します。次の表は、プル通知を使用してメールボックス イベントをサブスクライブする場合に、削除に対して返されるメールボックス イベントを示しています。  
  
**表 1: プル通知の削除に関連するメールボックス イベント**

|**削除の種類と EWS 操作**|**各フォルダーの識別子を指定する場合の Exchange 2010 の通知**|**すべてのフォルダー指定する場合の Exchange 2010 の通知**|**各フォルダーの識別子を指定する場合の Exchange Online と Exchange 2013 の通知**|**すべてのフォルダー指定する場合の Exchange Online と Exchange 2013**|
|:-----|:-----|:-----|:-----|:-----|
|[DeleteItem 操作](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)による削除済みアイテム フォルダーへの移動 <br/> |アイテムに対する DeletedEvent。  <br/> アイテムの親フォルダーに対する ModifiedEvent。  <br/> |アイテムに対する DeletedEvent。  <br/> アイテムの親フォルダーに対する ModifiedEvent。  <br/> |アイテムに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。アイテムはごみ箱の削除フォルダーに移動されます。  <br/> アイテムの親フォルダーに対する ModifiedEvent。  <br/> |アイテムに対する DeletedEvent。  <br/> 既定の検索フォルダー AllItems からのアイテムの DeletedEvent。  <br/> アイテムの親フォルダーに対する ModifiedEvent。  <br/> |
|[DeleteItem 操作](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)による物理的な削除 <br/> |アイテムに対する DeletedEvent。  <br/> アイテムの親フォルダーに対する ModifiedEvent。  <br/> |アイテムに対する DeletedEvent。  <br/> アイテムの親フォルダーに対する ModifiedEvent。  <br/> |アイテムに対する DeletedEvent。  <br/> アイテムの親フォルダーに対する ModifiedEvent。  <br/> |アイテムに対する DeletedEvent。  <br/> 既定の検索フォルダー AllItems からのアイテムの DeletedEvent。  <br/> アイテムの親フォルダーに対する ModifiedEvent。  <br/> |
|[DeleteItem 操作](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)による削除済みアイテム フォルダーへの移動 <br/> |アイテムに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。  <br/> アイテムの古い親フォルダーに対する ModifiedEvent。  <br/> 削除済みアイテム フォルダーである、アイテムの新しい親フォルダーに対する ModifiedEvent。  <br/> |アイテムに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。  <br/> アイテムの古い親フォルダーに対する ModifiedEvent。  <br/> 削除済みアイテム フォルダーである、アイテムの新しい親フォルダーに対する ModifiedEvent。  <br/> |アイテムに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。  <br/> アイテムの古い親フォルダーに対する ModifiedEvent。  <br/> 削除済みアイテム フォルダーである、アイテムの新しい親フォルダーに対する ModifiedEvent。  <br/> |既定の検索フォルダー AllItems からの DeletedEvent。  <br/> AllItems フォルダーのアイテムに対する CreatedEvent。  <br/> アイテムの元の親フォルダーに対する ModifiedEvent。  <br/> 削除済みアイテム フォルダーに対する ModifiedEvent。  <br/> |
|[DeleteFolder 操作](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)による削除済みアイテム フォルダーへの移動 <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに対する ModifiedEvent。  <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに対する ModifiedEvent。  <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに対する ModifiedEvent。  <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに対する ModifiedEvent。  <br/> |
|[DeleteFolder 操作](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)による物理的な削除 <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに対する ModifiedEvent。  <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに対する ModifiedEvent。  <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに対する ModifiedEvent。  <br/> |フォルダーに対する DeletedEvent。  <br/> フォルダーの親フォルダーに対する ModifiedEvent。  <br/> |
|[DeleteFolder 操作](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)による削除済みアイテム フォルダーへの移動。 <br/> |フォルダーに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。  <br/> フォルダーの古い親フォルダーに対する ModifiedEvent。  <br/> 削除済みアイテム フォルダーである、フォルダーの新しい親フォルダーに対する ModifiedEvent。  <br/> |フォルダーに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。  <br/> フォルダーの古い親フォルダーに対する ModifiedEvent。  <br/> 削除済みアイテム フォルダーである、フォルダーの新しい親フォルダーに対する ModifiedEvent。  <br/> |フォルダーに対する MovedEvent。これは、新旧両方の親フォルダー識別子を指定します。  <br/> フォルダーの古い親フォルダーに対する ModifiedEvent。  <br/> 削除済みアイテム フォルダーである、フォルダーの新しい親フォルダーに対する ModifiedEvent。  <br/> |フォルダーの古い親フォルダーに対する ModifiedEvent。  <br/> 削除済みアイテム フォルダーである、フォルダーの新しい親フォルダーに対する ModifiedEvent。  <br/> |
   
## <a name="see-also"></a>関連項目


- [Exchange の通知サブスクリプション、メールボックス イベント、および EWS](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Exchange で EWS を使用してアイテムを削除する](deleting-items-by-using-ews-in-exchange.md)
    
- [Exchange の EWS での削除に関連するエラーの処理](handling-deletion-related-errors-in-ews-in-exchange.md)
    

