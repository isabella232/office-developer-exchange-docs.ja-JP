---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: ReturnNewItemIds 要素は、新しいアイテムのアイテム識別子が応答で返されるかどうかを示します。
ms.openlocfilehash: 93ff4e37c56c3583e81711ba7e3582706d9ef940
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512381"
---
# <a name="returnnewitemids"></a>ReturnNewItemIds

**ReturnNewItemIds 要素** は、新しいアイテムのアイテム識別子が応答で返されるかどうかを示します。 
  
```XML
<ReturnNewItemIds/>
```

 **xs:boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CopyItem](copyitem.md) <br/> |アイテム ストア内のメールボックス内のアイテムをコピーする要求をExchangeします。  <br/> |
|[MoveItem](moveitem.md) <br/> |ストア内のアイテムを移動する要求をExchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

**ReturnNewItemIds** 要素のテキスト値 **が true** の場合、新しいアイテム識別子が応答で返されます。 false の **値は** 、新しいアイテム識別子が応答で返されないかどうかを示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

