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
description: 達成率の要素は、タスクの完了状態を表します。
ms.openlocfilehash: b7dd2f18bd3ef6addeb6d3a7b004510f35b9cb3d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456886"
---
# <a name="percentcomplete"></a>PercentComplete

**達成**率の要素は、タスクの完了状態を表します。 
  
```xml
<PercentComplete/>
```

 **再度**
## <a name="attributes-and-elements"></a>属性と要素

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

0 ~ 100 の整数を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

**達成**率を100に設定すると、 [completedate](completedate.md)要素を設定するか、 [Status](status.md)要素を**Completed**に設定した場合と同じ結果になります。 これらのプロパティの少なくとも2つを設定する要求では、最後に処理されたプロパティによって、これらの要素に設定されている値が決まります。 たとえば、**達成**率が100、 [completedate](completedate.md)が2007、[状態](status.md)が NotStarted で、プロパティがこの順序でストリーミングされている場合は、タスクの[状態](status.md)を NotStarted に、 [completedate](completedate.md)は**null**、**達成**率を0に設定することになります。 
  
この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[タスクの作成](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[タスクの削除](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

