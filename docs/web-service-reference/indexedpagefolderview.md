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
description: IndexedPageFolderView 要素がどのようにページングされたアイテム情報を説明 FindFolder 応答が返されます。
ms.openlocfilehash: f32f778daa6fa3fea93ab2bc1951f2407dcf7f80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831910"
---
# <a name="indexedpagefolderview"></a>IndexedPageFolderView

**IndexedPageFolderView**要素がどのようにページングされたアイテム情報を説明[FindFolder](findfolder.md)応答が返されます。 
  
[FindFolder](findfolder.md)
  
[IndexedPageFolderView](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |応答を取得するフォルダーの最大数について説明します。 この属性は、省略可能です。  <br/> |
|**Offset** <br/> |**ベース ポイント**からのオフセットを示します。 オフセットは、0 以上である必要があります。 **ベース ポイント**と等しい場合、開始オフセットが正の数値です。 **ベース ポイント**が終了する場合、オフセットが負の場合と処理されます。  <br/> これを識別するフォルダーは、応答で配信される最初のフォルダーになります。 この属性は、必要があります。  <br/> |
|**ベース ポイント** <br/> |フォルダーのページを開始または検索条件で検出されたフォルダーのセットの末尾から開始されるかどうかについて説明します。 末尾からのシークを常に検索を進めます。 この属性は、必要があります。  <br/> |
   
#### <a name="basepoint-attribute"></a>ベース ポイントの属性

|**値**|**説明**|
|:-----|:-----|
|先頭  <br/> |ページ ビューは、検索フォルダーのセットの先頭から開始されます。  <br/> |
|終了  <br/> |ページ ビューは、検索フォルダーのセットの末尾から開始します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを検索するための要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>備考

末尾からのシークでは、オフセットによって識別される原点に移動します。 さらに、ポインターが再び要求されたレコードの数によって。 などの場合は 100 個のレコードがある、オフセットが末尾から 25、75 から検索を開始します。 10 個のレコードが返された場合ポインターが逆方向、さらに 10 が 65 を記録し、65 75 からのレコードを返します。 次のインデックスは、64 です。 ページの末尾からの次のオフセットは、100-36 に相当する 64 です。 次のインデックス付きのページを取得する、末尾からの次のオフセットの値は、36 です。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

