---
title: SuppressReadReceipts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f0805560-7a2f-455b-94d2-ec4f1e3652c3
description: SuppressReadReceipts 要素は、開封確認を抑制する必要があるかどうかを示します。
ms.openlocfilehash: aa604d4907582bd73727ba664958a589a222f9cb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455934"
---
# <a name="suppressreadreceipts"></a>SuppressReadReceipts

**SuppressReadReceipts**要素は、開封確認を抑制する必要があるかどうかを示します。 
  
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

[ConversationAction](conversationaction.md)  | [Markallitemsasread](markallitemsasread.md)
  
## <a name="text-value"></a>テキスト値

**SuppressReadReciepts**要素のテキスト値が**true**である場合、開封確認が抑制されていることを示します。 値が**false**の場合、開封確認が送信者に送信されることを示します。 
  
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
   

