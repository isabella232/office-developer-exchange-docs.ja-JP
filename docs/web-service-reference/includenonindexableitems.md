---
title: IncludeNonIndexableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af7f202b-2889-447e-bdeb-aaad18ce6b46
description: IncludeNonIndexableItems 要素には、インデックスを作成できないアイテムを含めるかどうかを示すブール値が含まれています。
ms.openlocfilehash: ae91a3c6db82aea1d45940603d0ff2064d29f43f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831904"
---
# <a name="includenonindexableitems"></a>IncludeNonIndexableItems

**IncludeNonIndexableItems**要素には、インデックスを作成できないアイテムを含めるかどうかを示す**ブール**値が含まれています。 
  
```XML
<IncludeNonIndexableItems>true | false</IncludeNonIndexableItems>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **IncludeNonIndexableItems**要素のテキスト値は、インデックスを作成できないアイテムはメールボックスの保留リストに含まれていることを示します。 **False**の値は、メールボックスの保留リストにインデックスを作成できない項目が含まれていないことを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

