---
title: メッセージ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsFolder
api_type:
- schema
ms.assetid: 6c299de8-2087-4aeb-8e66-2bc7586509a6
description: メッセージ要素は、メールボックスに格納されている連絡先フォルダーを表します。
ms.openlocfilehash: 01302f00d84cfff9713e3b188b7799c537fc0629
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759681"
---
# <a name="contactsfolder"></a>メッセージ

**メッセージ**要素は、メールボックスに格納されている連絡先フォルダーを表します。 
  
```xml
<ContactsFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <EffectiveRights/>
   <SharingEffectiveRights/>
   <PermissionSet/>
</ContactsFolder>
```

 **ContactsFolderType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[フォルダー Id](folderid.md) <br/> |連絡先フォルダーの識別子と変更キーが含まれています。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |連絡先フォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[FolderClass](folderclass.md) <br/> |連絡先フォルダーのフォルダー クラスを表します。  <br/> |
|[表示名 (文字列)](displayname-string.md) <br/> |連絡先フォルダーの表示名が含まれています。  <br/> |
|[TotalCount](totalcount.md) <br/> |連絡先フォルダー内のアイテムの合計数を表します。  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |連絡先フォルダー内に含まれる子フォルダーの数を表します。 このプロパティは値の取得のみ可能です。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |連絡先フォルダーの拡張プロパティを識別します。  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |管理フォルダーに関する情報が含まれています。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。  <br/> |
|[SharingEffectiveRights (PermissionReadAccessType)](sharingeffectiverights-permissionreadaccesstype.md) <br/> |ユーザーが共有されている連絡先のデータを持っているアクセス許可を示します。  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |フォルダーに対して構成されているすべてのアクセス許可が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |[UpdateFolder 操作](updatefolder-operation.md)中にフォルダーのプロパティを追加するデータを指定します。  <br/> |
|[(集合的) を作成します。](create-foldersync.md) <br/> |ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |[UpdateFolder 操作](updatefolder-operation.md)でフォルダーの 1 つのプロパティには、更新プログラムを表します。  <br/> |
|[更新 (集合的)](update-foldersync.md) <br/> |ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。  <br/> |
|[フォルダー](folders-ex15websvcsotherref.md) <br/> |フォルダーの操作で使用されているフォルダーの配列が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

