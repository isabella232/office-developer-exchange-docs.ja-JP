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
description: CalendarPermission 要素は、予定表フォルダーにユーザーが持つアクセス権を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 7f6ceb6895add3fdd82cdd595463b3a80db822e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759591"
---
# <a name="calendarpermission"></a>CalendarPermission

**CalendarPermission**要素は、予定表フォルダーにユーザーが持つアクセス権を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarPermissionLevel](calendarpermissionlevel.md) <br/> |ユーザーが予定表フォルダーに必要なアクセス許可レベルを表します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[CanCreateItems](cancreateitems.md) <br/> |ユーザーがフォルダー内のアイテムを作成する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |ユーザーがフォルダーにサブフォルダーを作成する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[DeleteItems](deleteitems.md) <br/> |ユーザーがフォルダー内のアイテムを削除する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[EditItems](edititems.md) <br/> |ユーザーがフォルダー内のアイテムを編集する権限を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |ユーザーがフォルダーの連絡先であるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |ユーザーがフォルダーの所有者であるかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |ユーザーがフォルダーを表示できるかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ReadItems (CalendarPermissionType)](readitems-calendarpermissiontype.md) <br/> |ユーザーが予定表フォルダー内のアイテムの読み取りアクセス許可を持っているかどうかを示します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ユーザー Id](userid.md) <br/> |代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarPermissions](calendarpermissions.md) <br/> |フォルダーのアクセス許可を予定表の配列が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
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

