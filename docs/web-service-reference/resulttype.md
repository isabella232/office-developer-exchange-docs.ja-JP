---
title: 結果
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: 結果の要素には、実行する検索の種類が含まれています。 検索の種類では、統計情報のみをするしたり、のみをプレビューすることができます。
ms.openlocfilehash: 750f53ae05a7ad9f5aefc9396911a23ef32cdfc2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833211"
---
# <a name="resulttype"></a>結果

**結果**の要素には、実行する検索の種類が含まれています。 検索の種類では、統計情報のみをするしたり、のみをプレビューすることができます。 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 **SearchResultType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)
  
## <a name="text-value"></a>テキスト値

**結果**要素のテキスト値は、探索の検索で返される結果の型です。 **StatisticsOnly**のテキスト値では、検索の統計情報を返します。 **PreviewOnly**のテキスト値では、アイテムのプレビュー情報を返します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

