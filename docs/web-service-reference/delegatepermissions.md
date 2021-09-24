---
title: DelegatePermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DelegatePermissions
api_type:
- schema
ms.assetid: 292badc7-bab3-4368-9d7c-9a8b7edb279b
description: DelegatePermissions 要素には、ユーザーの代理人アクセス許可レベルの設定が含まれる。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: a8c7e06ae0ad4e1d12d06b559ad7d9f9468c4ade
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528993"
---
# <a name="delegatepermissions"></a>DelegatePermissions

**DelegatePermissions 要素には**、ユーザーの代理人アクセス許可レベルの設定が含まれる。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
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
|[CalendarFolderPermissionLevel](calendarfolderpermissionlevel.md) <br/> |既定の予定表フォルダーのアクセス許可が含まれる。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[TasksFolderPermissionLevel](tasksfolderpermissionlevel.md) <br/> |既定のタスク フォルダーのアクセス許可が含まれる。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[InboxFolderPermissionLevel](inboxfolderpermissionlevel.md) <br/> |既定の受信トレイ フォルダーのアクセス許可が含まれる。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[ContactsFolderPermissionLevel](contactsfolderpermissionlevel.md) <br/> |既定の連絡先フォルダーのアクセス許可が含まれる。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[NotesFolderPermissionLevel](notesfolderpermissionlevel.md) <br/> |既定の Notes フォルダーのアクセス許可が含まれる。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[JournalFolderPermissionLevel](journalfolderpermissionlevel.md) <br/> |既定のジャーナル フォルダーのアクセス許可が含まれる。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |メールボックスに追加または更新する 1 つの代理人を識別します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [AddDelegate 操作](adddelegate-operation.md) 
- [UpdateDelegate 操作](updatedelegate-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
- [代理人の追加](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

