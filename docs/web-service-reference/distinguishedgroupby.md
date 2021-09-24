---
title: DistinguishedGroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DistinguishedGroupBy
api_type:
- schema
ms.assetid: 6ff3ac48-02ba-40ec-a71b-c401bb2b127c
description: DistinguishedGroupBy 要素は、FindItem クエリの標準的なグループ化を提供します。
ms.openlocfilehash: 8b6001994603e49cd1c77288a93cfb9270d51e21
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511837"
---
# <a name="distinguishedgroupby"></a>DistinguishedGroupBy

**DistinguishedGroupBy** 要素は、FindItem クエリの標準的なグループ化を提供します。 
  
- [FindItem](finditem.md) 
- [DistinguishedGroupBy](distinguishedgroupby.md)
  
```xml
<DistinguishedGroupBy>
   <StandardGroupBy/>
</DistinguishedGroupBy>
```

 **DistinguishedGroupByType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[StandardGroupBy](standardgroupby.md) <br/> |グループ化された FindItem 操作の標準のグループ化および集計メカニズムを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索する要求を定義します。<br/><br/>次に、この要素の XPath 式を示します。  `/FindItem` <br/> |
   
## <a name="remarks"></a>注釈

**DistinguishedGroupBy** 要素は、結果がグループ化され、標準グループの 1 つがグループ化要件を満たしている場合に、FindItem 操作に追加できます。 **DistinguishedGroupBy 要素** も [GroupBy](groupby.md)要素も指定されていない場合、FindItem の結果はグループ化解除されます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [FindItem 操作](finditem-operation.md)
- [アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

