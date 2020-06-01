---
title: アクセス許可
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
description: Permission 要素は、ユーザーがフォルダーに対して持つアクセス許可を定義します。
ms.openlocfilehash: 0f7515dbb06f8423f8d4d95e1391496e8ac73653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459259"
---
# <a name="permission"></a>アクセス許可

Permission 要素は、ユーザーがフォルダーに対して持つアクセス**許可**を定義します。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[CanCreateItems](cancreateitems.md) <br/> |ユーザーがフォルダーにアイテムを作成する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |ユーザーがフォルダーにサブフォルダーを作成する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[DeleteItems](deleteitems.md) <br/> |ユーザーにフォルダー内のアイテムを削除する権限があるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[EditItems](edititems.md) <br/> |ユーザーにフォルダー内のアイテムを編集する権限があるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |ユーザーがフォルダーの連絡先であるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |ユーザーがフォルダーの所有者であるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |ユーザーがフォルダーを表示できるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[PermissionLevel](permissionlevel.md) <br/> |ユーザーがフォルダーに対して持っているアクセス許可の組み合わせを表します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ReadItems (PermissionType)](readitems-permissiontype.md) <br/> |ユーザーがフォルダー内のアイテムを読み取る権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[UserId](userid.md) <br/> |代理ユーザーまたはフォルダーのアクセス許可を持つユーザーを識別します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アクセス許可](permissions.md) <br/> |フォルダーに対して構成されているすべてのアクセス許可が含まれます。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
  
### <a name="version-differences"></a>バージョンの相違点

Exchange Online を対象とするアプリケーション、Office 365 の一部としての Exchange Online、または exchange 2013 以降のオンプレミスバージョンの Exchange の場合、フォルダーのアクセス許可は、 [Baseshape](baseshape.md)要素の値が[getfolder](getfolder-operation.md)操作要求で**allproperties**の値になっている場合は返されません。 フォルダーのアクセス許可を取得するには、 [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)要素を、 **Getfolder**要求の[additionalproperties](additionalproperties.md)要素に追加します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[フォルダーレベルのアクセス許可を設定する](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

