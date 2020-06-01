---
title: NonIndexableItemStatistic
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 593e0c79-9ec2-4040-a6a3-3c5c61cbdf7c
description: NonIndexableItemStatistic 要素には、インデックスを作成できないアイテムの1つの統計情報が含まれています。
ms.openlocfilehash: cc7bee9fd2759a16dd16538d6712e40ceb005fec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462683"
---
# <a name="nonindexableitemstatistic"></a>NonIndexableItemStatistic

**Nonindexableitemstatistic**要素には、インデックスを作成できないアイテムの1つの統計情報が含まれています。 
  
```XML
<NonIndexableItemStatistic>
   <Mailbox/>
   <ItemCount/>
   <ErrorMessage/>
</NonIndexableItemStatistic>
```

 **NonIndexableItemStatisticType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[メールボックス (文字列)](mailbox-string.md)  | [ItemCount](itemcount.md)  | [ErrorMessage](errormessage.md)
  
### <a name="parent-elements"></a>親要素

[NonIndexableItemStatistics](nonindexableitemstatistics.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |いいえ  <br/> |
   

