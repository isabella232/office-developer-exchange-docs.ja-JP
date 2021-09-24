---
title: SearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: SearchScope 要素は、検索の範囲を指定します。
ms.openlocfilehash: d4caa87cd552a633812b99d7e97f2419b156fb78
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523401"
---
# <a name="searchscope"></a>SearchScope

**SearchScope 要素** は、検索の範囲を指定します。 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 **MailboxSearchLocationType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[MailboxSearchScope](mailboxsearchscope.md)
  
## <a name="text-value"></a>テキスト値

SearchScope 要素の **テキスト値** は、探索検索で検索されるメールボックスの種類を示します。 **PrimaryOnly のテキスト値は**、プライマリ メールボックスが検索されたかどうかを示します。 **ArchiveOnly のテキスト値は**、アーカイブ メールボックスが検索されたかどうかを示します。 All のテキスト **値は** 、プライマリ メールボックスとアーカイブ メールボックスの両方が検索されるかどうかを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

