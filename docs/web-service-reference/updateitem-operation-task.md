---
title: UpdateItem 操作 (タスク)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: b0a7f114-d040-40eb-a8f3-05ea6489e472
description: UpdateItem 操作は、アイテム ストア内のタスク アイテムのプロパティを更新Exchangeされます。
ms.openlocfilehash: a268b4b281f149f14bc6c48a774fc9071093ebb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510751"
---
# <a name="updateitem-operation-task"></a>UpdateItem 操作 (タスク)

UpdateItem 操作は、アイテム ストア内のタスク アイテムのプロパティを更新Exchangeされます。
  
## <a name="remarks"></a>注釈

タスク要求を送信Exchange Web サービスを使用することはできません。 ExchangeWeb サービスは、MicrosoftOfficeOutlook によって作成されたタスク要求を返します。 タスク要求が既に送信されている場合、タスクを更新する要求はエラーを返します。
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a>定期的なタスクの現在の発生を更新する

定期的なタスクに対する UpdateItem 操作の結果は、単一の非回復タスクに対する UpdateItem 操作の結果とは異なります。 定期的なタスクの発生に対する変更により、次の更新が行われたときに一時タスクが生成されます。
  
1. 再生成または非再生成の繰り返しタスクの status プロパティは、Completed に **設定されます**。
    
2. リジェネラ処理されていない繰り返しタスクの開始日または終了日が変更されます。
    
たとえば **、UpdateItem** 要求で定期的なタスクの Completed 値が trueに設定されている場合 **、UpdateItemResponse** には、新しく作成された 1 回限定タスクを表す新しい Id と ChangeKey が含まれます。 要求に含まれる ID は引き続き有効であり、その ID で表される定期的なタスクが更新され、次に発生するタスクが表されます。 定期的なタスクが更新されたため、要求に含まれる ChangeKey が無効になります。 
  
GetItem 操作を [使用して、](getitem-operation.md) 定期的なタスクの **最新の ChangeKey** を取得できます。 
  
回復されていないタスクの場合、または定期的なタスクが最後に発生した場合、UpdateItem 応答は、そのタスクに渡されたのと同じ **ID** を返し、関連付けられた更新された **ChangeKey を返します**。
  
## <a name="see-also"></a>関連項目



[UpdateItem 操作](updateitem-operation.md)

