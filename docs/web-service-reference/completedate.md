---
title: CompleteDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: CompleteDate 要素は、アイテムが完了した日付を表します。
ms.openlocfilehash: 07f6034b4fd91d22ad07167d931bcd02a74782f9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518779"
---
# <a name="completedate"></a>CompleteDate

**CompleteDate 要素** は、アイテムが完了した日付を表します。 
  
```xml
<CompleteDate/>
```

 **DateTime**
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
|[Flag](flag.md) <br/> |メールボックス アイテムのフラグを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、日付と時刻を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

**CompleteDate の設定** は [、PercentComplete](percentcomplete.md)を 100 に設定するか、[状態] を [[完了](status.md)] に設定するのと **同じ効果があります**。 これらのプロパティのうち少なくとも 2 つを設定する要求では、最後に処理されたプロパティによって、これらの要素に設定される値が決定されます。 たとえば **、PercentComplete** が 100、CompleteDate が 2007 年 1 月 1 日 [、Status](status.md)が **NotStarted** の場合、プロパティは次 [](status.md)の順序でストリームされ、タスクの状態は **NotStarted、CompleteDate** は [](completedate.md)[null、PercentComplete](percentcomplete.md)は 0 に設定されます。 [](percentcomplete.md) 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
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

