---
title: SuppressReadReceipts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f0805560-7a2f-455b-94d2-ec4f1e3652c3
description: SuppressReadReceipts 要素は、読み取りレシートを抑制するかどうかを示します。
ms.openlocfilehash: 1f63f46f4e74a3123661caba39b737910bc2ef30
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517652"
---
# <a name="suppressreadreceipts"></a>SuppressReadReceipts

**SuppressReadReceipts 要素** は、読み取りレシートを抑制するかどうかを示します。 
  
```XML
<SuppressReadReceipts>true | false</SuppressReadReceipts>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[ConversationAction](conversationaction.md)  | [MarkAllItemsAsRead](markallitemsasread.md)
  
## <a name="text-value"></a>テキスト値

**SuppressReadReciepts** 要素のテキスト値 **が true** の場合、読み取りレシートが抑制されます。 false の **値は** 、読み取りレシートが送信者に送信されます。 
  
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
   

