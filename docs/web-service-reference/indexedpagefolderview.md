---
title: IndexedPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IndexedPageFolderView
api_type:
- schema
ms.assetid: c6dac232-244b-4db0-9a15-5e01b8aa7a7d
description: IndexedPageFolderView 要素は、ページ化されたアイテム情報が FindFolder 応答でどのように返されるのかについて説明します。
ms.openlocfilehash: 0a5d0f7e63549b7a851862d957ff32dff4333ce3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542240"
---
# <a name="indexedpagefolderview"></a>IndexedPageFolderView

**IndexedPageFolderView** 要素は、ページ化されたアイテム情報が [FindFolder](findfolder.md)応答でどのように返されるのかについて説明します。 
  
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
|**MaxEntriesReturned** <br/> |応答で返されるフォルダーの最大数を示します。 この属性は省略可能です。  <br/> |
|**Offset** <br/> |BasePoint からのオフセットについて **説明します**。 オフセットは 0 以上である必要があります。 **BasePoint が Beginning** に等しい場合、オフセットは正の値です。 **BasePoint が End** に等しい場合、オフセットは負の値である場合と同様に処理されます。  <br/> これは、応答で配信される最初のフォルダーになるフォルダーを識別します。 この属性は必須です。  <br/> |
|**BasePoint** <br/> |フォルダーのページが、検索条件で見つかった一連のフォルダーの開始または終了から開始するかどうかを示します。 最後からシークすると、常に後方に検索されます。 この属性は必須です。  <br/> |
   
#### <a name="basepoint-attribute"></a>BasePoint 属性

|**値**|**説明**|
|:-----|:-----|
|開始  <br/> |ページ ビューは、見つかったフォルダー セットの先頭から開始します。  <br/> |
|End  <br/> |ページ ビューは、見つかったフォルダー セットの末尾から開始します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを検索する要求を定義します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>注釈

端からシークするには、オフセットで識別される原点に移動します。 さらに、ポインターは要求されたレコードの数によって戻されます。 たとえば、レコードが 100 件で、オフセットが末尾から 25 の場合、検索は 75 から始まります。 10 レコードが返された場合、ポインターは追加の 10 レコードを 65 に戻し、レコード 65 から 75 を返します。 次のインデックスは 64 です。 ページの末尾からの次のオフセットは 100 ~ 64 で、36 に等しくなります。 次のインデックス付きページを取得する最後からの次のオフセットの値は 36 です。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

