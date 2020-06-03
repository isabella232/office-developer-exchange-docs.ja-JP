---
title: UserParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: UserParameters 要素には、有効と無効のクライアント拡張機能の一覧が含まれています。
ms.openlocfilehash: 76bf858adfb6d2ef76a25c234117131752c60d7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526754"
---
# <a name="userparameters"></a>UserParameters

**Userparameters**要素には、有効と無効のクライアント拡張機能の一覧が含まれています。 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 **GetClientExtensionUserParametersType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|UserId  <br/> |**UserId**属性のテキスト値は、ユーザーの識別子です。  <br/> |
|EnabledOnly  <br/> |**Enabledonly**テキスト値は、応答に有効な拡張機能のみが含まれているかどうかを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

[UserEnabledExtensions](userenabledextensions.md)  | [UserDisabledExtensions](userdisabledextensions.md)
  
### <a name="parent-elements"></a>親要素

[GetClientExtension](getclientextension.md)
  
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
   

