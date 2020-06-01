---
title: IndexedPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageFolderView
api_type:
- schema
ms.assetid: c6dac232-244b-4db0-9a15-5e01b8aa7a7d
description: IndexedPageFolderView 要素は、ページアイテムの情報が FindFolder 応答で返される方法を記述します。
ms.openlocfilehash: 6e9e2796c0bdcd9a15487f0e1bc7cbdf09d0a492
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457201"
---
# <a name="indexedpagefolderview"></a>IndexedPageFolderView

**Indexedpagefolderview**要素は、ページアイテムの情報が[findfolder](findfolder.md)応答で返される方法を記述します。 
  
[FindFolder](findfolder.md)
  
[IndexedPageFolderView](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |応答で返されるフォルダーの最大数を表します。 この属性は省略可能です。  <br/> |
|**Offset** <br/> |**BasePoint**からのオフセットを記述します。 オフセットは0以上である必要があります。 **BasePoint**が先頭と等しい場合、オフセットは正になります。 **BasePoint**が End と等しい場合、オフセットは負の値として処理されます。  <br/> これにより、どのフォルダーが応答で配信される最初のフォルダーになるかを識別します。 この属性は必須です。  <br/> |
|**BasePoint** <br/> |フォルダーのページが検索条件に一致する一連のフォルダーの先頭から開始するか、または末尾から開始するかを指定します。 末尾からシークすると、常に逆方向に検索されます。 この属性は必須です。  <br/> |
   
#### <a name="basepoint-attribute"></a>BasePoint 属性

|**値**|**説明**|
|:-----|:-----|
|始まる  <br/> |ページビューは、見つかったフォルダーセットの先頭から開始されます。  <br/> |
|End  <br/> |ページビューは、見つかったフォルダーセットの末尾から開始されます。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを検索する要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>注釈

End からシークするには、オフセットで識別される起点に移動する必要があります。 さらに、要求されたレコードの数だけポインターが戻されます。 たとえば、100レコードがあり、オフセットが最後から25である場合、検索は75から開始されます。 10件のレコードが返された場合、ポインターは10レコード後ろに65に移動され、レコード 65 ~ 75 を返します。 次のインデックスは64です。 ページの最後からの次のオフセットは、36と等しい 100-64 です。 次のインデックス付きページを取得するために、末尾からの次のオフセットの値は36です。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

