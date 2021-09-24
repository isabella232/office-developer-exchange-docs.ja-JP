---
title: 状態
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Status
api_type:
- schema
ms.assetid: 80121e41-291b-4fc0-a55e-6f677d4b5fb5
description: Status 要素は、タスク アイテムの状態を表します。
ms.openlocfilehash: 5ec50e3f0c06ad3ec8301ddbe8e7bd249b1e8fe9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525541"
---
# <a name="status"></a>状態

**Status 要素** は、タスク アイテムの状態を表します。 
  
```xml
<Status/>
```

 **TaskStatusType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[タスク](task.md) <br/> |ストア内のタスクをExchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 この要素で使用できるテキスト値を次に示します。
  
- NotStarted
    
- InProgress
    
- 完了
    
- WaitingOnOthers
    
- Deferred
    
## <a name="remarks"></a>注釈

[CompleteDate の設定](completedate.md)は [、PercentComplete](percentcomplete.md)を 100 に設定するか、[状態] を [**完了**] に設定するのと **同じ効果があります**。 これらのプロパティのうち少なくとも 2 つを設定する要求では、最後に処理されたプロパティによって、これらの要素に設定される値が決定されます。 たとえば、PercentComplete が 100 の場合 **、CompleteDate** は 1/1/2007 で **、Status** は NotStarted で、プロパティは次の順序でストリーミングされます。その効果は、タスクの Status を **NotStarted、CompleteDate** を **null、PercentComplete** を 0 に設定します。   
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[タスクの作成](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[タスクの削除](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

