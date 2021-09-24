---
title: Restriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Restriction
api_type:
- schema
ms.assetid: 77f19014-d112-4999-8e83-ecc32a117a73
description: Restriction 要素は、FindItem/FindFolder および検索フォルダー操作でアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。
ms.openlocfilehash: 378c2d0ce7911638e5e58346de46759e7fdd87f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540567"
---
# <a name="restriction"></a>Restriction

**Restriction 要素は**、FindItem/FindFolder および検索フォルダー操作でアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。 
  
```xml
<Restriction>
   <SearchExpression/>
</Restriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[And](and.md) <br/> |2 つ以上の検索式の間で **ブール型 AND** 演算を実行できる検索式を表します。  <br/> |
|[Contains](contains.md) <br/> |指定したプロパティに指定された定数文字列値が含まれているかどうかを決定する検索式を表します。  <br/> |
|[Excludes](excludes.md) <br/> |プロパティのビットのマスクを実行します。  <br/> |
|[Exists](exists.md) <br/> |指定されたプロパティがアイテムに存在する場合に **true** を返す検索式を表します。  <br/> |
|[IsEqualTo](isequalto.md) <br/> |プロパティと定数値または別のプロパティを比較し、等しい場合は **true** と評価される検索式を表します。  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |プロパティを定数値または別のプロパティと比較する検索式を表し、最初のプロパティが値またはプロパティより大きい場合は **true** を返します。  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |プロパティを定数値または別のプロパティと比較する検索式を表し、最初のプロパティが値またはプロパティ以上の場合は **true** を返します。  <br/> |
|[IsLessThan](islessthan.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが値またはプロパティより小さい場合は **true** を返す検索式を表します。  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが値またはプロパティ以下の場合は **true** を返す検索式を表します。  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |定数値または別のプロパティとプロパティを比較する検索式を表し、値が同じではない場合は **true** を返します。  <br/> |
|[Not](not.md) <br/> |含まれる検索式のブール値をネゲートする検索式を表します。  <br/> |
|[Or](or.md) <br/> |含まれる検索式に対して論理 **OR** 操作を実行する検索式を表します。 **Or 要素は**、その子 **が true** を返す場合に true を返 **します**。  <br/> |
|[SearchExpression](searchexpression.md) <br/> |制限内の置換された要素を表します。 この要素は、XML インスタンス ドキュメントでは使用されません。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを識別するための要求を定義します。  <br/> |
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索する要求を定義します。  <br/> |
|[SearchParameters](searchparameters.md) <br/> |検索フォルダーを定義するパラメーターを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

