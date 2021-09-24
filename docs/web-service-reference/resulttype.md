---
title: ResultType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: ResultType 要素には、実行する検索の種類が含まれる。 検索の種類は統計のみ、またはプレビューのみ可能です。
ms.openlocfilehash: 65227a8f79a7abd597653b646a7c3985c3e38ac9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509456"
---
# <a name="resulttype"></a>ResultType

**ResultType 要素** には、実行する検索の種類が含まれる。 検索の種類は統計のみ、またはプレビューのみ可能です。 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 **SearchResultType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SearchMailboxesResult](searchmailboxesresult.md)  | [SearchMailboxes](searchmailboxes.md)
  
## <a name="text-value"></a>テキスト値

ResultType 要素の **テキスト値** は、探索検索で返される結果の種類です。 **StatisticsOnly のテキスト値は、** 検索統計を返します。 **PreviewOnly のテキスト値は、** アイテムのプレビュー情報を返します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

