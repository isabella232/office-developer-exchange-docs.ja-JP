---
title: PrintAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7232505a-bab0-4d78-87bc-6cc4b568937a
description: PrintAllowed 要素は、印刷が有効になっているかどうかを指定します。
ms.openlocfilehash: 85c18f3a6bd8f1705d0e21b99bae15484348f777
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832880"
---
# <a name="printallowed"></a>PrintAllowed

**PrintAllowed**要素は、印刷が有効になっているかどうかを指定します。 
  
```XML
<PrintAllowed> true | false </PrintAllowed>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[RightsManagementLicenseData](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **PrintAllowed**要素のテキスト値は、権限管理の対象項目の内容の印刷を許可することを示します。 **False**の値は、印刷が許可されていないことを示します。 
  
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
   

