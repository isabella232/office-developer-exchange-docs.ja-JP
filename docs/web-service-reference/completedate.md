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
description: CompleteDate 要素は、項目が完了された日付を表します。
ms.openlocfilehash: 00a1ec25be737ec0a5cc874063e1bce19a96cee0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759635"
---
# <a name="completedate"></a>CompleteDate

**CompleteDate**要素は、項目が完了された日付を表します。 
  
```xml
<CompleteDate/>
```

 **DateTime**
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
|[Flag](flag.md) <br/> |メールボックス アイテムにフラグを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

日付と時刻を表すテキスト値は、この要素を使用する場合に必要です。
  
## <a name="remarks"></a>備考

**CompleteDate**を設定すると、[達成率](percentcomplete.md)を 100 または**完了**[状態](status.md)に設定すると同じ効果になります。 で、これらのプロパティには、少なくとも 2 つ設定、処理された最後のプロパティ値が決まります。 これらの要素に設定されている要求。 たとえば、[達成率](percentcomplete.md)は、100、 **CompleteDate**には、2007 年 1 月 1 日[状態](status.md)が [**未開始**、しプロパティをこの順序でストリームは、影響がある**未開始にタスクの[ステータス](status.md)を設定するのには**、 [CompleteDate](completedate.md) **null**、および[達成率](percentcomplete.md)を 0 にするです。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
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

