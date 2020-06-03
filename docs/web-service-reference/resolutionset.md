---
title: 解像度セット
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolutionSet
api_type:
- schema
ms.assetid: 43d5b876-0e87-4414-9b1d-bff1c1ec825c
description: 解像度セット要素には、あいまいな名前の解決の配列が含まれています。
ms.openlocfilehash: 483a096a7fcedbabe25758ebcaa31c83405a0ad4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467173"
---
# <a name="resolutionset"></a>解像度セット

解像度**セット**要素には、あいまいな名前の解決の配列が含まれています。 
  
[ResolveNamesResponse](resolvenamesresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
  
[解像度セット](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 **Arrayof解像度の種類**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |インデックス付きのページビューを使用している場合に、次の要求に使用する必要がある次のインデックスを表します。  <br/> |
|**NumeratorOffset** <br/> |分数のページビューを使用しているときに、次の要求に対して使用する新しい分子の値を表します。  <br/> |
|**AbsoluteDenominator** <br/> |分数のページビューを使用しているときに、次の要求に対して使用する次の分母を表します。  <br/> |
|**IncludesLastItemInRange** <br/> |現在の結果にクエリの最後のアイテムが含まれている場合は、この属性は true になり、追加のページングは必要ありません。  <br/> |
|**TotalItemsInView** <br/> |ビュー内のアイテムの合計数を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Resolution](resolution.md) <br/> |1つの解決済みエンティティを含みます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |ResolveNames 要求の状態と結果を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

**解像度セット**要素には、最大100個の解決済みエンティティを含めることができます。 
  
この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[ResolveNames](resolvenames.md)
  
[ResolveNamesResponse](resolvenamesresponse.md)
  
[ResolveNames 操作](resolvenames-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

