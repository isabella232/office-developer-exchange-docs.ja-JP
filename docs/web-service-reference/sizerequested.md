---
title: SizeRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e86f98b6-83b5-4530-80eb-dc5df42e2c62
description: SizeRequested 要素には、GetUserPhoto 操作で要求された写真サイズが含まれる。
ms.openlocfilehash: 799869a85d7f72e79753a73f9c259388a2702bf5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545917"
---
# <a name="sizerequested"></a>SizeRequested

**SizeRequested 要素には****、GetUserPhoto** 操作で要求された写真サイズが含まれる。 
  
```XML
<SizeRequested>HR48x48 | HR64x64 | HR96X96 | HR120X120 | HR240X240 | HR360X360 | HR432X432 | HR504X504 | HR648X648</SizeRequested>
```

 **UserPhotoSizeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[GetUserPhoto](getuserphoto.md)
  
## <a name="text-value"></a>テキスト値

**SizeRequested 要素のテキスト** 値は、サーバーから返されるデジタル 画像の要求された写真サイズです。 次の表は **、SizeRequested 要素のテキスト値を示** しています。 
  
|**値**|**意味**|
|:-----|:-----|
|HR48x48  <br/> |画像の高さは 48 ピクセル、幅は 48 ピクセルです。  <br/> |
|HR64x64  <br/> |画像の高さは 64 ピクセル、幅は 64 ピクセルです。  <br/> |
|HR96x96  <br/> |画像の高さは 96 ピクセル、幅は 96 ピクセルです。  <br/> |
|HR120x120  <br/> |画像の高さは 120 ピクセル、幅は 120 ピクセルです。  <br/> |
|HR240x240  <br/> |画像の高さは 240 ピクセル、幅は 240 ピクセルです。  <br/> |
|HR360x360  <br/> |画像の高さは 360 ピクセル、幅は 360 ピクセルです。  <br/> |
|HR432x432  <br/> |画像の高さは 432 ピクセル、幅は 432 ピクセルです。  <br/> |
|HR504x504  <br/> |画像の高さは 504 ピクセル、幅は 504 ピクセルです。  <br/> |
|HR648x648  <br/> |画像の高さは 648 ピクセル、幅は 648 ピクセルです。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> ||
   

