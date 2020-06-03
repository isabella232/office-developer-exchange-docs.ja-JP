---
title: CalendarPermission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermission
api_type:
- schema
ms.assetid: 3aafb221-a04b-41f6-804e-eda810f1ba28
description: CalendarPermission 要素は、ユーザーが予定表フォルダーに対して持つアクセス権を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: c43f75e6cf5abc2dce9af6c04122ec9a589dcd58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529477"
---
# <a name="calendarpermission"></a>CalendarPermission

**Calendarpermission**要素は、ユーザーが予定表フォルダーに対して持つアクセス権を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<Permission>
   <CalendarPermissionLevel/>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 **CalendarPermissionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[CalendarPermissionLevel](calendarpermissionlevel.md) <br/> |ユーザーが予定表フォルダーに対して持っているアクセス許可レベルを表します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[CanCreateItems](cancreateitems.md) <br/> |ユーザーがフォルダーにアイテムを作成する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |ユーザーがフォルダーにサブフォルダーを作成する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[DeleteItems](deleteitems.md) <br/> |ユーザーにフォルダー内のアイテムを削除する権限があるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[EditItems](edititems.md) <br/> |ユーザーにフォルダー内のアイテムを編集する権限があるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |ユーザーがフォルダーの連絡先であるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |ユーザーがフォルダーの所有者であるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |ユーザーがフォルダーを表示できるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ReadItems (CalendarPermissionType)](readitems-calendarpermissiontype.md) <br/> |ユーザーが予定表フォルダー内のアイテムを読み取る権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[UserId](userid.md) <br/> |代理ユーザーまたはフォルダーのアクセス許可を持つユーザーを識別します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarPermissions](calendarpermissions.md) <br/> |フォルダーに対する予定表のアクセス許可の配列を格納します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
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

