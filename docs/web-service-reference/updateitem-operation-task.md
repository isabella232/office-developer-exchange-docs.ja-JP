---
title: UpdateItem 操作 (タスク)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: b0a7f114-d040-40eb-a8f3-05ea6489e472
description: UpdateItem 操作は、Exchange ストア内のタスクアイテムのプロパティを更新するために使用されます。
ms.openlocfilehash: 0041af114d11fd9577037dd154e40b84e8483c35
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459806"
---
# <a name="updateitem-operation-task"></a>UpdateItem 操作 (タスク)

UpdateItem 操作は、Exchange ストア内のタスクアイテムのプロパティを更新するために使用されます。
  
## <a name="remarks"></a>注釈

Exchange Web サービスを使用してタスクの要求を送信することはできません。 Exchange Web サービスは、Microsoft office outlook によって作成されたタスク要求を返すことができます。 タスクの依頼が既に送信されている場合、タスクを更新する要求はエラーを返します。
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a>定期的なタスクの現在の発生を更新する

定期的なタスクに対する UpdateItem 操作の結果は、単一の非定期的なタスクに対する UpdateItem 操作の結果とは異なります。 定期的なタスクの発生に変更を加えると、次の更新が行われたときに1回限りのタスクが生成されます。
  
1. [再生成] または [再生成なし] のタスクの [状態] プロパティは、[**完了**] に設定されています。
    
2. 再生成以外のタスクの開始日または終了日が変更されています。
    
たとえば、 **Updateitem**要求で定期的なタスクの完了値を**true**に設定すると、 **updateitemresponse**には、新しく作成された1回限りのタスクを表す新しい Id と changekey が含まれます。 要求に含まれていた Id は依然として有効であり、その Id で表される定期タスクは、次の出現を表すように更新されています。 要求に含まれていた ChangeKey は、定期タスクが更新されているため無効になりました。 
  
[GetItem 操作](getitem-operation.md)を使用して、定期的なタスクの最新の**changekey**を取得できます。 
  
非定期的なタスクまたは定期的なタスクの最後の発生の場合、UpdateItem 応答は渡されたものと同じ**Id**を返し、関連付けられた更新された**changekey**を返します。
  
## <a name="see-also"></a>関連項目




  [UpdateItem 操作](updateitem-operation.md)

