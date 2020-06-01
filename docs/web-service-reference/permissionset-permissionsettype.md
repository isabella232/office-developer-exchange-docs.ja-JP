---
title: PermissionSet (PermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d
description: PermissionSet 要素には、フォルダーに対して構成されているすべてのアクセス許可が含まれています。
ms.openlocfilehash: 5639ee8ba64742f39c0274f4e3aaa76d75bea42b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468132"
---
# <a name="permissionset-permissionsettype"></a>PermissionSet (PermissionSetType)

**PermissionSet**要素には、フォルダーに対して構成されているすべてのアクセス許可が含まれています。 
  
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
|[アクセス許可](permissions.md) <br/> |フォルダーのアクセス許可のコレクションを格納します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[UnknownEntries](unknownentries.md) <br/> |Active Directory ディレクトリサービスに対して解決できない不明なエントリの配列が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |作成、取得、検索、同期、更新を行うフォルダーを定義します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックスに含まれている検索フォルダーを表します。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックスに含まれている連絡先フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックスに含まれる tasks フォルダーを表します。  <br/> |
   
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

