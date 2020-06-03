---
title: DelegatePermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegatePermissions
api_type:
- schema
ms.assetid: 292badc7-bab3-4368-9d7c-9a8b7edb279b
description: DelegatePermissions 要素には、ユーザーの代理アクセス許可レベルの設定が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 2cf8c9a8d3c5db8e13d43c207df173c12fca5acb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457411"
---
# <a name="delegatepermissions"></a>DelegatePermissions

**DelegatePermissions**要素には、ユーザーの代理アクセス許可レベルの設定が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<DelegatePermissions>
   <CalendarFolderPermissionLevel/>
   <TasksFolderPermissionLevel/>
   <InboxFolderPermissionLevel/>
   <ContactsFolderPermissionLevel/>
   <NotesFolderPermissionLevel/>
   <JournalFolderPermissionLevel/>
</DelegatePermissions>
```

**DelegatePermissionsType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[CalendarFolderPermissionLevel](calendarfolderpermissionlevel.md) <br/> |既定の予定表フォルダーのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[タスク Folderpermissionlevel](tasksfolderpermissionlevel.md) <br/> |既定のタスクフォルダーのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[受信トレイフォルダーの Permissionlevel](inboxfolderpermissionlevel.md) <br/> |既定の受信トレイフォルダーのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ContactsFolderPermissionLevel](contactsfolderpermissionlevel.md) <br/> |既定の連絡先フォルダーのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[注釈 Folderpermissionlevel](notesfolderpermissionlevel.md) <br/> |既定のメモフォルダーのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[JournalFolderPermissionLevel](journalfolderpermissionlevel.md) <br/> |既定の履歴フォルダーのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |メールボックスに追加または更新する単一の代理人を指定します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
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

- [AddDelegate 操作](adddelegate-operation.md) 
- [UpdateDelegate 操作](updatedelegate-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [代理人の追加](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

