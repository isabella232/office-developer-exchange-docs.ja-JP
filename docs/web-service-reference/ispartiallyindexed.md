---
title: Ispartiのインデックス付き
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 542e7b90-eafe-4711-a9d7-71bbc30d9646
description: Isparti"Indexed/インデックス" 要素は、アイテムが部分的にインデックス付けされているかどうかを示します。
ms.openlocfilehash: 4bf0c3e5dd7b75a90ac087958fbceda334306af1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466487"
---
# <a name="ispartiallyindexed"></a>Ispartiのインデックス付き

**Isparti"indexed/インデックス**" 要素は、アイテムが部分的にインデックス付けされているかどうかを示します。 
  
```XML
<IsPartiallyIndexed>true | false</IsPartiallyIndexed>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[NonIndexableItemDetail](nonindexableitemdetail.md)
  
## <a name="text-value"></a>テキスト値

**Ispartithe indexed**要素のテキスト値が**true の場合**は、メールボックスアイテムが部分的にインデックス付けされていることを示します。 値が**false**の場合は、メールボックスアイテムが部分的にインデックス付けされていないことを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

