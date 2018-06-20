---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: ReturnNewItemIds 要素は、新しい項目の項目の識別子が応答で返されるかどうかを示します。
ms.openlocfilehash: 6d3bc83c05a82d6e448041167676f41c2620dcd4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833232"
---
# <a name="returnnewitemids"></a>ReturnNewItemIds

**ReturnNewItemIds**要素は、新しい項目の項目の識別子が応答で返されるかどうかを示します。 
  
```XML
<ReturnNewItemIds/>
```

 **xs:boolean**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CopyItem](copyitem.md) <br/> |Exchange ストア内のメールボックスにアイテムをコピーするための要求を定義します。  <br/> |
|[MoveItem](moveitem.md) <br/> |Exchange ストア内のアイテムを移動する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **ReturnNewItemIds**要素のテキスト値は、応答に新しいアイテムの識別子が返されることを示します。 **False**の値は、応答に新しいアイテムの識別子が返されないことを示します。 
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

