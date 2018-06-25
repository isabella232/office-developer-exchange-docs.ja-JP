---
title: ModifyRecipientsAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f25e673-0df0-4285-bf03-a083a395cdab
description: ModifyRecipientsAllowed 要素は、受信者の変更が有効になっているかどうかを指定します。
ms.openlocfilehash: 2b07c7fa8e6b5872621c8b019b60584abbf98e3c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832473"
---
# <a name="modifyrecipientsallowed"></a>ModifyRecipientsAllowed

**ModifyRecipientsAllowed**要素は、受信者の変更が有効になっているかどうかを指定します。 
  
```XML
<ModifyRecipientsAllowed> true | false </ModifyRecipientsAllowed>
```

 **boolean**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[RightsManagementLicenseData](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **ModifyRecipientsAllowed**要素のテキスト値は、項目の受信者リストが権限管理を有効にするとアイテムを変更できることを示します。 **False**の値は、受信者の一覧が変更可能ではないことを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   

