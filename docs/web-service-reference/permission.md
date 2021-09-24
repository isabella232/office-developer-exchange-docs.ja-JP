---
title: アクセス許可
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Permission
api_type:
- schema
ms.assetid: b8d0429a-0e58-4480-9847-4901970c7033
description: Permission 要素は、ユーザーがフォルダーに対して持つアクセスを定義します。
ms.openlocfilehash: bc3e140aaf7bd9ea7f1a4993c9bea1dcad8d39fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512668"
---
# <a name="permission"></a>アクセス許可

**Permission 要素** は、ユーザーがフォルダーに対して持つアクセスを定義します。 
  
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
|[CanCreateItems](cancreateitems.md) <br/> |ユーザーがフォルダー内にアイテムを作成する権限を持つかどうかを示します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |ユーザーがフォルダーにサブフォルダーを作成する権限を持つかどうかを示します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[DeleteItems](deleteitems.md) <br/> |ユーザーがフォルダー内のアイテムを削除する権限を持つかどうかを示します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[EditItems](edititems.md) <br/> |ユーザーがフォルダー内のアイテムを編集する権限を持つかどうかを示します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |ユーザーがフォルダーの連絡先であるかどうかを示します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |ユーザーがフォルダーの所有者であるかどうかを示します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |ユーザーがフォルダーを表示できるかどうかを示します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[PermissionLevel](permissionlevel.md) <br/> |ユーザーがフォルダーに対して持つアクセス許可の組み合わせを表します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[ReadItems (PermissionType)](readitems-permissiontype.md) <br/> |ユーザーがフォルダー内のアイテムを読み取る権限を持つかどうかを示します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[UserId](userid.md) <br/> |代理人ユーザーまたはフォルダー アクセス許可を持つユーザーを識別します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アクセス許可](permissions.md) <br/> |フォルダーに対して構成済みのすべてのアクセス許可が含まれる。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は、Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
  
### <a name="version-differences"></a>バージョンの相違点

Office 365 の一部として Exchange Online、Exchange Online、または Exchange 2013 から始まるオンプレミスバージョンの Exchange を対象とするアプリケーションの場合 [、BaseShape](baseshape.md)要素に [GetFolder](getfolder-operation.md)の **AllProperties** の値がある場合、フォルダーのアクセス許可は返されません。操作要求。 フォルダーのアクセス許可を取得するには、GetFolder 要求の [AdditionalProperties](additionalproperties.md)要素に [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md)要素 **を追加** します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[アクセス許可Folder-Level設定する](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

