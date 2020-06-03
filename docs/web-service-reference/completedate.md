---
title: CompleteDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: CompleteDate 要素は、アイテムが完了した日付を表します。
ms.openlocfilehash: fff3d5d3105bf63c9cdd34cbcf828d57ca287b86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461423"
---
# <a name="completedate"></a>CompleteDate

**Completedate**要素は、アイテムが完了した日付を表します。 
  
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
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[Flag](flag.md) <br/> |メールボックスアイテムのフラグを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、日付と時刻を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

**Completedate**の設定は、[達成](percentcomplete.md)率を100または[状態](status.md)から**完了**に設定した場合と同じ効果があります。 これらのプロパティの少なくとも2つを設定する要求では、最後に処理されたプロパティによって、これらの要素に設定されている値が決まります。 たとえば、[達成](percentcomplete.md)率が100、 **completedate**が2007、[状態](status.md)が**NotStarted**で、プロパティがその順序でストリーミングされている場合は、タスクの[状態](status.md)を**NotStarted**に設定し、 [completedate](completedate.md)を**null**に設定し、[達成](percentcomplete.md)率を0に設定することになります。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
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

