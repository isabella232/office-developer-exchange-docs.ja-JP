---
title: ResolutionSet
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
description: ResolutionSet 要素には、あいまいな名前の解決策の配列が含まれています。
ms.openlocfilehash: ad7bd31c85051e8c80aea25aa9e6f2914cf0ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833160"
---
# <a name="resolutionset"></a>ResolutionSet

**ResolutionSet**要素には、あいまいな名前の解決策の配列が含まれています。 
  
[ResolveNamesResponse](resolvenamesresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
  
[ResolutionSet](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 **ArrayOfResolutionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |次に、インデックス付きページング ビューを使用しているときに次の要求に使用するインデックスを表します。  <br/> |
|**NumeratorOffset** <br/> |分数のページ ビューを使用しているときに、次の要求に使用する新しい分子の値を表します。  <br/> |
|**AbsoluteDenominator** <br/> |分母分数のページ ビューを使用しているときに、次の要求に使用するを表します。  <br/> |
|**IncludesLastItemInRange** <br/> |追加のページングが必要ないように、この属性が true の場合、現在の結果には、クエリの最後の項目が含まれているされます。  <br/> |
|**TotalItemsInView** <br/> |ビュー内の項目の合計数を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[解決策](resolution.md) <br/> |解決された 1 つのエンティティが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |ResolveNames 要求の結果ステータスを格納します。  <br/> |
   
## <a name="remarks"></a>備考

**ResolutionSet**要素には、100 の解決されたエンティティの最大を含めることができます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[ResolveNames](resolvenames.md)
  
[ResolveNamesResponse](resolvenamesresponse.md)
  
[ResolveNames 操作](resolvenames-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

