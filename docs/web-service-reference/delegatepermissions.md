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
description: DelegatePermissions 要素には、ユーザーの代理人アクセス許可レベルの設定が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 319592b6c3386a07b3094115c335c7fb8ffe1130
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759950"
---
# <a name="delegatepermissions"></a>DelegatePermissions

**DelegatePermissions**要素には、ユーザーの代理人アクセス許可レベルの設定が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarFolderPermissionLevel](calendarfolderpermissionlevel.md) <br/> |既定の予定表フォルダーのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[TasksFolderPermissionLevel](tasksfolderpermissionlevel.md) <br/> |既定の作業フォルダーのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[InboxFolderPermissionLevel](inboxfolderpermissionlevel.md) <br/> |既定の受信トレイ フォルダーのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ContactsFolderPermissionLevel](contactsfolderpermissionlevel.md) <br/> |既定の連絡先フォルダーのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[NotesFolderPermissionLevel](notesfolderpermissionlevel.md) <br/> |既定のメモ フォルダーのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[JournalFolderPermissionLevel](journalfolderpermissionlevel.md) <br/> |仕訳帳の既定のフォルダーのアクセス許可が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |1 つのデリゲートを追加するメールボックスの更新を識別します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
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

- [AddDelegate 操作](adddelegate-operation.md) 
- [UpdateDelegate 操作](updatedelegate-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [デリゲートを追加します。](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

