---
title: SizeRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e86f98b6-83b5-4530-80eb-dc5df42e2c62
description: SizeRequested 要素には、GetUserPhoto 操作に対して要求された写真のサイズが含まれています。
ms.openlocfilehash: 2e79bbb158fa9a22cbd3ec08fcd6e60429e113b4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460457"
---
# <a name="sizerequested"></a>SizeRequested

**SizeRequested**要素には、 **getuserphoto**操作に対して要求された写真のサイズが含まれています。 
  
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

**SizeRequested**要素のテキスト値は、サーバーから返されるデジタルイメージの要求された写真のサイズです。 次の表は、 **SizeRequested**要素のテキスト値を示しています。 
  
|**値**|**意味**|
|:-----|:-----|
|HR48x48  <br/> |画像の幅は48ピクセル、高さは48ピクセルです。  <br/> |
|HR64x64  <br/> |画像の幅は64ピクセル、高さは64ピクセルです。  <br/> |
|HR96x96  <br/> |画像の幅は96ピクセル、高さは96ピクセルです。  <br/> |
|HR120x120  <br/> |画像の幅は120ピクセル、高さは120ピクセルです。  <br/> |
|HR240x240  <br/> |画像の幅は240ピクセル、高さは240ピクセルです。  <br/> |
|HR360x360  <br/> |画像の幅は360ピクセル、高さは360ピクセルです。  <br/> |
|HR432x432  <br/> |画像の幅は432ピクセル、高さは432ピクセルです。  <br/> |
|HR504x504  <br/> |画像の幅は504ピクセル、高さは504ピクセルです。  <br/> |
|HR648x648  <br/> |画像の幅は648ピクセル、高さは648ピクセルです。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> ||
   

