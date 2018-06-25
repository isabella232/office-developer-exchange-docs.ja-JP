---
title: RootFolder (FindItemResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 187e009f-efaa-42a8-8962-329a645213ab
description: RootFolder 要素には、FindItem 操作時に単一のルート フォルダーの検索の結果が含まれています。
ms.openlocfilehash: ea17369ef4efc4112a738b430c8f0dbab3886341
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833254"
---
# <a name="rootfolder-finditemresponsemessage"></a>RootFolder (FindItemResponseMessage)

**RootFolder**要素には、 [FindItem 操作](finditem-operation.md)中に単一のルート フォルダーの検索の結果が含まれています。
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 **FindItemParentType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |インデックス付きページング ビューを使用する場合、次の要求に使用する必要があります次のインデックスを表します。  <br/> |
|**NumeratorOffset** <br/> |分数のページ ビューを使用するときに、次の要求に使用する新しい分子の値を表します。  <br/> |
|**AbsoluteDenominator** <br/> |分数形式のページングを実行する場合、次の要求に使用する分母を表します。  <br/> |
|**IncludesLastItemInRange** <br/> |さらにページングが必要ないように、現在の結果が、クエリの最後の項目を含めるかどうかを示します。  <br/> |
|**TotalItemsInView** <br/> |制限を満たすアイテムの総数を表します。 グループ化された[FindItem 操作](finditem-operation.md)では、 **TotalItemsInView**属性は、ビュー内の項目の合計数とグループ数の合計を返します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Items](items.md) <br/> |見つかったアイテムの配列が含まれています[FindItem 操作](finditem-operation.md)要求で指定された検索条件があります。  <br/> |
|[グループ](groups.md) <br/> |検出されたグループのコレクションが含まれています[FindItem 操作](finditem-operation.md)要求で指定された検索と集計の基準が存在します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |[FindItem 操作](finditem-operation.md)要求の結果ステータスを格納します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindItem 操作](finditem-operation.md)
  
[IndexedPagingOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[NumeratorOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[AbsoluteDenominator](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[IncludesLastItemInRange](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[TotalItemsInView](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[項目を検索します。](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

