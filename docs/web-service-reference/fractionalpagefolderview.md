---
title: FractionalPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: FractionalPageFolderView 要素は、ページ ビューの開始位置と FindFolder 要求で返されるフォルダーの最大数を示します。
ms.openlocfilehash: b3d4bd63f94c2db7761dabfad1e32558ceb30be5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530254"
---
# <a name="fractionalpagefolderview"></a>FractionalPageFolderView

**FractionalPageFolderView** 要素は、ページ ビューの開始位置と [FindFolder](findfolder.md)要求で返されるフォルダーの最大数を示します。 
  
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
|**MaxEntriesReturned** <br/> |[FindFolder](findfolder.md)応答で返される結果の最大数を識別します。 この属性は省略可能です。  <br/> |
|**Numerator** <br/> |結果セットの開始位置からの小数部のオフセットの分子を表します。 この属性は必須です。 分子は分母以下である必要があります。 この属性は、0 以上の整数値を表す必要があります。 詳細については、このトピックの「備考」を参照してください。  <br/> |
|**分母** <br/> |結果セット内のフォルダーの総数の開始位置からの分母を表します。 この属性は必須です。 この属性は、1 より大きい整数値を表す必要があります。 詳細については、このトピックの「備考」を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを識別するための要求を定義します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>注釈

見つかったフォルダーのセットの開始位置からのページ ビューのオフセットは、分数で表されます。 分数は **、Numerator** 属性と **分** 母属性によって定義され、情報のページの開始場所を示します。 たとえば **、Numerator** が 4、分母が 5 に等しい場合、返される情報のページは、結果セットへの 5 分の 4 の位置にあるエントリから始まります。 
  
分数が 0 に評価される場合、結果セットの開始を示します。 分数が 1 に評価される場合、結果セットの終わりを示します。
  
> [!NOTE]
> 分数はページの開始点を表し、結果セットの結果の数は返されません。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindFolder 操作](findfolder-operation.md)


[フォルダーの検索](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

