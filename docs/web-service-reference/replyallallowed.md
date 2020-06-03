---
title: ReplyAllAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d22f68cf-b18b-45d0-a9ff-414b7db0e67e
description: ReplyAllAllowed 要素は、すべての返信を権限管理データに対して許可するかどうかを指定します。
ms.openlocfilehash: 56dfe7670ed87581999bfe0a340bcc72c99d04ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467915"
---
# <a name="replyallallowed"></a>ReplyAllAllowed

**ReplyAllAllowed**要素は、すべての返信を権限管理データに対して許可するかどうかを指定します。 
  
```XML
<ReplyAllAllowed> true | false </ReplyAllAllowed>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[RightsManagementLicenseData](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a>テキスト値

**ReplyAllAllowed**要素のテキスト値が**true**の場合は、すべての返信が権限管理データに対して許可されていることを示します。 値が**false**の場合は、全員に返信が許可されていないことを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

