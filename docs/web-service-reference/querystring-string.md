---
title: QueryString (String)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: QueryString 要素は、FindPeople 操作要求のクエリ文字列と一致する値のセットを指定します。 QueryString が指定されていない検索では、指定したフォルダーのすべてのアイテムが返されます。
ms.openlocfilehash: 6dfd4b5552511e2551baf5ce645f82d4f74e5499
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523735"
---
# <a name="querystring-string"></a>QueryString (String)

**QueryString 要素は**[、FindPeople](findpeople-operation.md)操作要求のクエリ文字列と一致する値のセットを指定します。 QueryString が指定 **されていない検索では** 、指定したフォルダーのすべてのアイテムが返されます。 
  
```XML
<QueryString/> 
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindPeople](findpeople.md) <br/> |[FindPeople 操作検索の引数を格納](findpeople-operation.md)します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**QueryString テキスト** 値は、高度なクエリ構文 [(AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx)のサブセットを使用して行われたメールボックス クエリを表します。 この要素の構文の詳細については [、「QueryString (QueryStringType)」を参照してください](querystring-querystringtype.md)。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindPeople 操作](findpeople-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

