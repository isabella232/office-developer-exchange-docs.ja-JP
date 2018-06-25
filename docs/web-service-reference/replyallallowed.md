---
title: ReplyAllAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d22f68cf-b18b-45d0-a9ff-414b7db0e67e
description: ReplyAllAllowed 要素は、権限の許可は、すべての応答でデータを管理するかどうかを指定します。
ms.openlocfilehash: cf814e6f27a734afc51b633bf832126a57d7ca5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833105"
---
# <a name="replyallallowed"></a>ReplyAllAllowed

**ReplyAllAllowed**要素は、権限の許可は、すべての応答でデータを管理するかどうかを指定します。 
  
```XML
<ReplyAllAllowed> true | false </ReplyAllAllowed>
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

の**場合は true** 、 **ReplyAllAllowed**要素のテキスト値は、権限の許可は、すべての応答にデータが管理されていることを示します。 **False**の値は、すべての返信が許可されていないことを示します。 
  
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
   

