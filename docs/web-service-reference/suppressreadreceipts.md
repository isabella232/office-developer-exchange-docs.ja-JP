---
title: SuppressReadReceipts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f0805560-7a2f-455b-94d2-ec4f1e3652c3
description: 要素では、開封確認をするかどうかを示す SuppressReadReceipts を抑制する必要があります。
ms.openlocfilehash: 794252da6b3e6b6e6f36181c1811a2a001bfaf53
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839630"
---
# <a name="suppressreadreceipts"></a>SuppressReadReceipts

**SuppressReadReceipts**要素を示す確認メッセージを抑制するかを読み取るかどうか。 
  
```XML
<SuppressReadReceipts>true | false</SuppressReadReceipts>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)
  
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **SuppressReadReciepts**要素のテキスト値では、読み取り確認メッセージが抑制されていることを示します。 **False**の値は、読み取り受信確認を送信者に送信されますを示します。 
  
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
   

