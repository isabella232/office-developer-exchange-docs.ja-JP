---
title: UpdateItem 処理 (タスク)
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
description: UpdateItem 操作を使用して、Exchange ストア内の作業項目のプロパティを更新します。
ms.openlocfilehash: d6f966fa663300b476383a136d30cf611d6bfb9b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839864"
---
# <a name="updateitem-operation-task"></a>UpdateItem 処理 (タスク)

UpdateItem 操作を使用して、Exchange ストア内の作業項目のプロパティを更新します。
  
## <a name="remarks"></a>備考

仕事の依頼を送信するのに Exchange Web サービスを使用することはできません。 Exchange Web サービスでは、MicrosoftOfficeOutlook によって作成された仕事の依頼を返すことができます。 仕事の依頼は既に送信された場合、タスクの更新要求はエラーを返します。
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a>定期的な仕事の現在の回を更新

定期的なタスクに対して UpdateItem 操作の結果は、1 つの非定期的なタスクで UpdateItem 演算の結果によって異なります。 定期的な仕事の発生への変更には、次の更新が行われたときに生成される一時的な仕事が発生します。
  
1. 再生成するか、nonregenerating の定期的なタスクの status プロパティは、**完了**に設定されます。
    
2. 開始日または nonregenerating の定期的なタスクの終了日が変更されます。
    
たとえば、 **UpdateItem**要求は、定期的なタスクの完了] の値を**true**にしている場合は、 **UpdateItemResponse**は、新しい Id と変更キーを新しく作成された 1 回限りのタスクを表す含まれます。 要求に含まれていた Id がまだ有効であると、次の出現箇所を表示するのにはその Id で表される定期的なタスクが更新されました。 定期タスクが更新されたために、要求に含まれていた変更キーは有効ではありません。 
  
[GetItem 操作](getitem-operation.md)を使用すると、定期タスクの最新の**変更キー**を取得します。 
  
非定期的なタスクまたは定期タスクの最後に出現 UpdateItem 応答は、渡されたものとそれに関連付けられた**変更キー**の更新を取得する同じ**Id**を返します。
  
## <a name="see-also"></a>関連項目




  [UpdateItem 操作](updateitem-operation.md)

