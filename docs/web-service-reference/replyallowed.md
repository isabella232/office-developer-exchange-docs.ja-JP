---
title: ReplyAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 880af57e-0fa1-473c-b87c-f02f1133ba5e
description: ReplyAllowed 要素は、応答を許可するか権限の管理対象のデータを指定します。
ms.openlocfilehash: c774836ac6e72648d6a6c017d41fcafdb64d116c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833107"
---
# <a name="replyallowed"></a>ReplyAllowed

**ReplyAllowed**要素は、応答を許可するか権限の管理対象のデータを指定します。 
  
```XML
<ReplyAllowed> true | false </ReplyAllowed>
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

の**場合は true** 、 **ReplyAllowed**要素のテキスト値は、返信を許可する権限の管理対象のデータを示します。 **False**の値は、返信が許可されていないことを示します。 
  
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
   

