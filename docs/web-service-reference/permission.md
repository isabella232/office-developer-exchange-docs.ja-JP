---
title: Permission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Permission
api_type:
- schema
ms.assetid: b8d0429a-0e58-4480-9847-4901970c7033
description: アクセス許可要素では、フォルダーにユーザーが持つアクセス権を定義します。
ms.openlocfilehash: 600d60f481c4f1d407c3a39ab65d6ddcf46d04e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832735"
---
# <a name="permission"></a>アクセス許可

**アクセス許可**要素では、フォルダーにユーザーが持つアクセス権を定義します。 
  
```XML
<Permission>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <PermissionLevel/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 **PermissionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[CanCreateItems](cancreateitems.md) <br/> |ユーザーがフォルダー内のアイテムを作成する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |ユーザーがフォルダーにサブフォルダーを作成する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[DeleteItems](deleteitems.md) <br/> |ユーザーがフォルダー内のアイテムを削除する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[EditItems](edititems.md) <br/> |ユーザーがフォルダー内のアイテムを編集する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |ユーザーがフォルダーの連絡先であるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |ユーザーがフォルダーの所有者であるかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |ユーザーがフォルダーを表示できるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[PermissionLevel](permissionlevel.md) <br/> |フォルダーにユーザーが持つアクセス許可の組み合わせを表します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ReadItems (PermissionType)](readitems-permissiontype.md) <br/> |ユーザーがフォルダー内のアイテムの読み取りアクセス許可を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ユーザー Id](userid.md) <br/> |代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アクセス許可](permissions.md) <br/> |フォルダーに対して構成されているすべてのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
  
### <a name="version-differences"></a>バージョンの相違点

アプリケーションを対象とする Exchange のオンライン、Office 365 の一部として Exchange のオンライン、または、設置型バージョンの Exchange から Exchange 2013 では、フォルダーのアクセス許可は返されません[BaseShape](baseshape.md)の要素に**AllProperties**の値が設定されている場合[GetFolder](getfolder-operation.md)操作要求します。 フォルダーのアクセス許可を取得するには、 **GetFolder**要求内の[AdditionalProperties](additionalproperties.md)要素に[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)の要素を追加します。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[フォルダー レベルのアクセス許可の設定](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

