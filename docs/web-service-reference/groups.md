---
title: グループ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Groups
api_type:
- schema
ms.assetid: 6b6b2d67-219d-4dfb-a4ed-d627b1cfb33f
description: グループ要素には、FindItem 操作の要求で指定されている検索と集計の基準で検出されたグループのコレクションが含まれています。
ms.openlocfilehash: 406a1974899e89243f52ba7a56afcc172c4f3df6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831786"
---
# <a name="groups"></a>グループ

**グループ**要素には、 [FindItem 操作](finditem-operation.md)要求で指定されている検索と集計の基準で検出されたグループのコレクションが含まれています。 
  
```xml
<Groups>
   <GroupedItems/>
</Groups>
```

 **ArrayOfGroupedItemsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[GroupedItems](groupeditems.md) <br/> |グループ化された[FindItem 操作](finditem-operation.md)の結果であるアイテムのコレクションを呼び出します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |[FindItem 操作](finditem-operation.md)の処理中に単一のルート フォルダーの検索の結果が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

結果内の異なるグループごとに 1 つの[GroupedItems](groupeditems.md)インスタンスが発生します。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindItem 操作](finditem-operation.md)


[項目を検索します。](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

