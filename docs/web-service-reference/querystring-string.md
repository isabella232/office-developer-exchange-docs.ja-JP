---
title: クエリ文字列 (文字列)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: クエリ文字列要素は、FindPeople の操作要求のクエリ文字列に一致する返される値のセットを指定します。 指定なしのクエリ文字列の検索は、指定したフォルダーからすべての項目を返します。
ms.openlocfilehash: 9c5c733adcec1496e36986fd720b56b0a0274593
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832935"
---
# <a name="querystring-string"></a>クエリ文字列 (文字列)

**クエリ文字列**要素は、 [FindPeople 操作](findpeople-operation.md)の要求のクエリ文字列に一致する返される値のセットを指定します。 指定されていない**クエリ文字列**の検索は、指定したフォルダーからすべての項目を返します。 
  
```XML
<QueryString/> 
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindPeople](findpeople.md) <br/> |[FindPeople 操作](findpeople-operation.md)の検索の引数が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

**クエリ文字列**のテキスト値では、[高度なクエリ構文 (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx)のサブセットを使用してメールボックスのクエリを表します。 この要素の構文については、[クエリ文字列 (QueryStringType)](querystring-querystringtype.md)を参照してください。
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[FindPeople 操作](findpeople-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

