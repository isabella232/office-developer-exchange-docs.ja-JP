---
title: PolicyTipsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 16409652-21e4-4bd3-9373-67e1882236b4
description: PolicyTipsEnabled 要素は、ポリシーのヒントが有効になっているかどうかを示します。
ms.openlocfilehash: 683131a5cefd6757faf582324f312b01fd9ddb33
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832838"
---
# <a name="policytipsenabled"></a>PolicyTipsEnabled

**PolicyTipsEnabled**要素は、ポリシーのヒントが有効になっているかどうかを示します。 
  
```XML
<PolicyTipsEnabled> true | false </PolicyTipsEnabled>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md)
  
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **PolicyTipsEnabled**要素のテキスト値は、メールボックスのポリシーのヒントが有効であることを示します。 **False**の値は、メールボックスに対して、ポリシー ヒントが無効になっていることを示します。 
  
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
   

