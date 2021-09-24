---
title: UserParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: UserParameters 要素には、有効なクライアント拡張機能と無効になっているクライアント拡張機能の一覧が含まれる。
ms.openlocfilehash: 1d93ec0f4e44b238fcb9aca23672c262795290a6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510730"
---
# <a name="userparameters"></a>UserParameters

**UserParameters 要素** には、有効なクライアント拡張機能と無効になっているクライアント拡張機能の一覧が含まれる。 
  
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
|UserId  <br/> |UserId 属性の **テキスト値** は、ユーザーの識別子です。  <br/> |
|EnabledOnly  <br/> |**EnabledOnly のテキスト値は**、応答に有効な拡張機能のみを含むかどうかを示します。  <br/> |
   
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
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

