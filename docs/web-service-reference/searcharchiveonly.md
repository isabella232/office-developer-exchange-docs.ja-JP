---
title: SearchArchiveOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cce5344c-b622-44d4-bc14-a0de346c9335
description: SearchArchiveOnly 要素は、インデックス付けされていないアイテムに対してアーカイブメールボックスのみを検索するかどうかを示します。
ms.openlocfilehash: 9014044ed06c697cc43dd62103d7a1a907bda5a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460499"
---
# <a name="searcharchiveonly"></a>SearchArchiveOnly

**SearchArchiveOnly**要素は、インデックス付けされていないアイテムに対してアーカイブメールボックスのみを検索するかどうかを示します。 
  
```xml
<SearchArchiveOnly>true | false</SearchArchiveOnly>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Getnonindexableitemstatistics](getnonindexableitemstatistics.md) │ [getnonindexableitemstatistics](getnonindexableitemdetails.md)
  
## <a name="text-value"></a>テキスト値

**SearchArchiveOnly**要素のテキスト値が**true**の場合、インデックス付けされていないアイテムの検索はアーカイブメールボックスでのみ実行されることを示します。 テキスト値が**false**の場合は、検索がプライマリメールボックスとアーカイブメールボックスに対して実行されることを示します。 
  
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
   

