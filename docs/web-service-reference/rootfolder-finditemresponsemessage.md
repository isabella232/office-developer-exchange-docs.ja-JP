---
title: RootFolder (FindItemResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 187e009f-efaa-42a8-8962-329a645213ab
description: RootFolder 要素には、FindItem 操作中に 1 つのルート フォルダーを検索した結果が含まれる。
ms.openlocfilehash: 96fa9e162dde34394e7c34543dd25a6f018ae7de
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527538"
---
# <a name="rootfolder-finditemresponsemessage"></a>RootFolder (FindItemResponseMessage)

**RootFolder 要素には**、FindItem 操作中に 1 つのルート フォルダーを検索した [結果が含まれる。](finditem-operation.md)
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 **FindItemParentType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |インデックス付きページング ビューを使用するときに次の要求に使用する次のインデックスを表します。  <br/> |
|**NumeratorOffset** <br/> |分数ページ ビューを使用する場合に次の要求に使用する新しい分子値を表します。  <br/> |
|**AbsoluteDenominator** <br/> |分数ページングを実行するときに次の要求に使用する次の分母を表します。  <br/> |
|**IncludesLastItemInRange** <br/> |現在の結果にクエリの最後の項目が含まれているかどうかを示します。この場合、それ以上のページングは不要です。  <br/> |
|**TotalItemsInView** <br/> |制限に合格するアイテムの総数を表します。 グループ化された [FindItem](finditem-operation.md)操作では **、TotalItemsInView** 属性はビュー内のアイテムの総数とグループの総数を返します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Items](items.md) <br/> |FindItem 操作要求で識別される検索条件を持つ、見つかったアイテムの [配列を格納](finditem-operation.md) します。  <br/> |
|[グループ](groups.md) <br/> |FindItem 操作要求で識別される検索および集計条件を持つグループのコレクション [が含](finditem-operation.md) まれます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |FindItem 操作要求の状態と結果 [を格納](finditem-operation.md) します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindItem 操作](finditem-operation.md)
  
[IndexedPagingOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[NumeratorOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[AbsoluteDenominator](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[IncludesLastItemInRange](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[TotalItemsInView](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

