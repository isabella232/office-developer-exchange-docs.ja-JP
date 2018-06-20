---
title: OptedInto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 083a23d9-acc3-4c15-9d30-c20bf7e6808d
description: OptedInto 要素は、リテンション ・ ポリシーをユーザーが有効にするかどうかを示すブール値を指定します。
ms.openlocfilehash: 0d8fb2b07c6c98ba6973ab6efabe9c35d2d1ac12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832657"
---
# <a name="optedinto"></a>OptedInto

**OptedInto**要素は、リテンション ・ ポリシーをユーザーが有効にするかどうかを示すブール値を指定します。 
  
```XML
<OptedInto>true | false</OptedInto>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **OptedInto**要素のテキスト値は、保持ポリシーにユーザーが有効にことを示します。 **False**の値は、リテンション ・ ポリシーに、ユーザーを選択しなかったことを示します。 
  
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
   

