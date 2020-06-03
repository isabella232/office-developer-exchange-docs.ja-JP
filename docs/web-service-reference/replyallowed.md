---
title: ReplyAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 880af57e-0fa1-473c-b87c-f02f1133ba5e
description: ReplyAllowed 要素は、権限管理データに対して返信を許可するかどうかを指定します。
ms.openlocfilehash: f9aa97fc5d85837323d6d9e3e1e13c7b9fd11715
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529862"
---
# <a name="replyallowed"></a>ReplyAllowed

**ReplyAllowed**要素は、権限管理データに対して返信を許可するかどうかを指定します。 
  
```XML
<ReplyAllowed> true | false </ReplyAllowed>
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

**ReplyAllowed**要素のテキスト値が**true**の場合は、権限管理データに対して返信が許可されていることを示します。 値が**false**の場合は、返信が許可されていないことを示します。 
  
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
   

