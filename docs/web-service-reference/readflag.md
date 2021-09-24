---
title: ReadFlag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9d91aa89-9f9f-4877-846d-aaf48bbeec7c
description: ReadFlag 要素は、フォルダー内のアイテムに設定する読み取り状態を示します。
ms.openlocfilehash: ac079f6adbdb2686221dd52d748b05ac4141d6c6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523651"
---
# <a name="readflag"></a>ReadFlag

**ReadFlag 要素** は、フォルダー内のアイテムに設定する読み取り状態を示します。 
  
```XML
<ReadFlag>true | false</ReadFlag>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[MarkAllItemsAsRead](markallitemsasread.md)
  
## <a name="text-value"></a>テキスト値

**ReadFlag** 要素 **のテキスト値が true** の場合は、フォルダー内のアイテムが読み取りとしてマークされます。 false の **値は** 、フォルダー内のアイテムが未読としてマークされます。 
  
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
   

