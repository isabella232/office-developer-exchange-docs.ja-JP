---
title: FractionalPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: FractionalPageFolderView 要素は、ページビューの開始位置と、FindFolder 要求で返されるフォルダーの最大数を示します。
ms.openlocfilehash: a8627c6277b49655d3933679128b844118633cda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463070"
---
# <a name="fractionalpagefolderview"></a>FractionalPageFolderView

**FractionalPageFolderView**要素は、ページビューの開始位置と、 [findfolder](findfolder.md)要求で返されるフォルダーの最大数を示します。 
  
[FindFolder](findfolder.md)
  
[FractionalPageFolderView](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |[Findfolder](findfolder.md)応答で返される結果の最大数を指定します。 この属性は省略可能です。  <br/> |
|**分子** <br/> |結果セットの先頭からの、分数のオフセットの分子を表します。 この属性は必須です。 分子は、分母以下の値である必要があります。 この属性は、ゼロ以上の整数値を表す必要があります。 詳細については、このトピックで後述する「備考」を参照してください。  <br/> |
|**分母** <br/> |結果セット内のフォルダーの総数の先頭からの、分単位のオフセットの分母を表します。 この属性は必須です。 この属性は、1より大きい整数値を表す必要があります。 詳細については、このトピックで後述する「備考」を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを識別する要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>注釈

検索されたフォルダーのセットの先頭からのページビューオフセットは、分数で示されます。 **分子**および**分母**属性で定義されている分数は、情報のページが開始する場所を示します。 たとえば、**分子**が4で、**分母**が5の場合、返された情報のページは、結果セット内の fifths にあるエントリから始まります。 
  
分数が0に評価された場合は、結果セットの開始を示します。 分数が1に評価される場合は、結果セットの末尾を示します。
  
> [!NOTE]
> 分数は、結果セット内の結果の数ではなく、ページの開始点を表します。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[FindFolder 操作](findfolder-operation.md)


[フォルダーの検索](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

