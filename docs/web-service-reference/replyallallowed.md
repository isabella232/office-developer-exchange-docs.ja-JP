---
title: ReplyAllAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d22f68cf-b18b-45d0-a9ff-414b7db0e67e
description: ReplyAllAllowed 要素は、権限管理データに対してすべての返信を許可するかどうかを指定します。
ms.openlocfilehash: 56b383e4273ca78ee291eeb658d69873109593f3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523595"
---
# <a name="replyallallowed"></a>ReplyAllAllowed

**ReplyAllAllowed 要素** は、権限管理データに対してすべての返信を許可するかどうかを指定します。 
  
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

**ReplyAllAllowed** 要素のテキスト値 **が true** の場合、権限管理データに対してすべての返信が許可されます。 false の **値は** 、返信のすべてが許可されていない状態を示します。 
  
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
   

