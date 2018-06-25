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
description: FractionalPageFolderView 要素は、ページ ビューが起動し、フォルダーの最大数は、FindFolder 要求で返されるについて説明します。
ms.openlocfilehash: 3cb5f8333634a0c484ae3ce6a6256631cff57cc5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760589"
---
# <a name="fractionalpagefolderview"></a>FractionalPageFolderView

**FractionalPageFolderView**要素は、ページ ビューが起動し、フォルダーの最大数は、 [FindFolder](findfolder.md)要求で返されるについて説明します。 
  
[FindFolder](findfolder.md)
  
[FractionalPageFolderView](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |[FindFolder](findfolder.md)の応答で返す結果の最大数を指定します。 この属性は、省略可能です。  <br/> |
|**分子** <br/> |結果セットの先頭からのオフセットを表す分数の分子を表します。 この属性は、必要があります。 分子は分母となる以下にする必要があります。 この属性は、0 以上である整数値を表す必要があります。 詳細については、このトピックの後半の「解説」を参照してください。  <br/> |
|**分母** <br/> |結果セット内のフォルダーの合計数の先頭からのオフセットを表す分数の分母を表します。 この属性は、必要があります。 この属性が 1 より大きい整数値を表す必要があります。 詳細については、このトピックの後半の「解説」を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを識別するための要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>備考

検出されたフォルダーのセットの先頭からのページ ビュー オフセットは、分数で表されます。 分数の**分子**と**分母**の属性によって定義されているは、情報のページを開始する位置について説明します。 などの**分子**が 4 と等しいし、**分母**を"5"と等しい、エントリで返される情報の開始ページには 5 分の 4 つの結果セットにする方法が配置されています。 
  
割合は、0 に評価されると、結果セットの先頭を示します。 分数を 1 つに評価する場合、結果セットの末尾を示します。
  
> [!NOTE]
> 分数は、ページの開始位置を表す、結果セットにどのように多くの結果が返されます。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindFolder 操作](findfolder-operation.md)


[フォルダーを検索します。](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

