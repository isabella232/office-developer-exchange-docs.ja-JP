---
title: PermissionSet (PermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d
description: PermissionSet 要素には、フォルダーに対して構成されているすべてのアクセス許可が含まれる。
ms.openlocfilehash: b18fef33d3be6cb8c525f731a264860c3a83afdc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543143"
---
# <a name="permissionset-permissionsettype"></a>PermissionSet (PermissionSetType)

**PermissionSet 要素** には、フォルダーに対して構成されているすべてのアクセス許可が含まれる。 
  
```XML
<PermissionSet>
   <Permissions/>
   <UnknownEntries/>
</PermissionSet>
```

 **PermissionSetType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[アクセス許可](permissions.md) <br/> |フォルダーのアクセス許可のコレクションを格納します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[UnknownEntries](unknownentries.md) <br/> |Active Directory ディレクトリ サービスに対して解決できない不明なエントリの配列が含まれます。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |作成、取得、検索、同期、または更新するフォルダーを定義します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックスに含まれる検索フォルダーを表します。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックスに含まれる連絡先フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックスに含まれるタスク フォルダーを表します。  <br/> |
   
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

