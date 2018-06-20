---
title: SizeRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e86f98b6-83b5-4530-80eb-dc5df42e2c62
description: SizeRequested 要素には、GetUserPhoto 操作の要求された写真のサイズが含まれています。
ms.openlocfilehash: 43e422512b1e8f06e410e533e9ae1dc49283d5f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833504"
---
# <a name="sizerequested"></a>SizeRequested

**SizeRequested**要素には、 **GetUserPhoto**操作の要求された写真のサイズが含まれています。 
  
```XML
<SizeRequested>HR48x48 | HR64x64 | HR96X96 | HR120X120 | HR240X240 | HR360X360 | HR432X432 | HR504X504 | HR648X648</SizeRequested>
```

 **UserPhotoSizeType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[GetUserPhoto](getuserphoto.md)
  
## <a name="text-value"></a>テキスト値

**SizeRequested**要素のテキスト値は、サーバーから返されるデジタル画像の写真を要求されたサイズです。 次の表は、 **SizeRequested**要素のテキスト値を識別します。 
  
|**値**|**意味**|
|:-----|:-----|
|HR48x48  <br/> |イメージは、48 ピクセル、高さと幅 48 ピクセルです。  <br/> |
|HR64x64  <br/> |イメージは 64 ピクセル、高さと幅は 64 ピクセルです。  <br/> |
|HR96x96  <br/> |イメージは、96 ピクセル、高さと幅が 96 ピクセルです。  <br/> |
|HR120x120  <br/> |イメージは、120 ピクセル、高さと幅が 120 ピクセルです。  <br/> |
|HR240x240  <br/> |イメージは、高さ 240 ピクセル、幅 240 ピクセルです。  <br/> |
|HR360x360  <br/> |イメージは 360 ピクセル、高さと幅が 360 ピクセルです。  <br/> |
|HR432x432  <br/> |イメージは、432 ピクセル、高さと幅 432 ピクセルです。  <br/> |
|HR504x504  <br/> |イメージは、504 ピクセル、高さと幅は 504 ピクセルです。  <br/> |
|HR648x648  <br/> |イメージは、648 ピクセル、高さと幅が 648 ピクセルです。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> ||
   

