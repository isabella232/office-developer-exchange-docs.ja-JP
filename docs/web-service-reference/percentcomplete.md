---
title: PercentComplete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PercentComplete
api_type:
- schema
ms.assetid: 58a67f8a-c4dc-42dc-97ae-a9e5cc672d2d
description: 達成率の要素は、タスクの完了状態を説明します。
ms.openlocfilehash: 18e53221ecdf60df195445ed7692c03795bdcc1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832717"
---
# <a name="percentcomplete"></a>PercentComplete

**達成率**の要素は、タスクの完了状態を説明します。 
  
```xml
<PercentComplete/>
```

 **二重**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

0 から 100 までの整数を表す文字列値は、必要があります。
  
## <a name="remarks"></a>備考

[CompleteDate](completedate.md)要素を設定または**完了**の[状態](status.md)の要素の設定と同じ効果を**達成率**を 100 に設定します。 で、これらのプロパティには、少なくとも 2 つ設定、処理された最後のプロパティ値が決まります。 これらの要素に設定されている要求。 たとえば、**達成率**は、100、 [CompleteDate](completedate.md)には、2007 年 1 月 1 日[状態](status.md)が [未開始、し、プロパティがこの順序でストリーム配信、影響がある未開始、[に、タスクの[ステータス](status.md)を設定するのにはCompleteDate](completedate.md)は**null**との**達成率**を 0 にします。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[タスクを作成します。](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[タスクを削除します。](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

