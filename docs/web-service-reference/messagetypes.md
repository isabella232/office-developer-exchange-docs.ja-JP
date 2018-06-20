---
title: MessageTypes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fac1cfe0-8e7b-4196-b3ad-4e86043d9c9b
description: MessageTypes 要素は、検索するメッセージの配列を指定します。
ms.openlocfilehash: 0dca94def0e919ea2a12487b374392a8b80275cb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832461"
---
# <a name="messagetypes"></a>MessageTypes

**MessageTypes**要素は、検索するメッセージの配列を指定します。 
  
```XML
<MessageTypes>
   <SearchItemKind/>
</MessageTypes>
```

 **ArrayOfSearchItemKindsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[SearchItemKind](searchitemkind.md)
  
### <a name="parent-elements"></a>親要素

[FindMailboxStatisticsByKeywords](findmailboxstatisticsbykeywords.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> ||
   

