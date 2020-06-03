---
title: Get-managementrole
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a5ee3299-1b2c-4a2a-9fe4-997febc7267a
description: ManagementRole 要素は、ユーザーおよびアプリケーションの管理役割のリストを指定します。
ms.openlocfilehash: 4e4ac1b38869d3c5dabe142c63b2aac9477036fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44450915"
---
# <a name="managementrole"></a>Get-managementrole

**Managementrole**要素は、ユーザーおよびアプリケーションの管理役割のリストを指定します。 
  
```XML
<ManagementRole>
   <UserRoles/>
   <ApplicationRoles/>
</ManagementRole>
```

 **ManagementRoleType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[Userroles](userroles.md)  | [Applicationroles](applicationroles.md)
  
### <a name="parent-elements"></a>親要素

なし。
  
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
   

