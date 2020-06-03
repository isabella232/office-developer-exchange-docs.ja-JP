---
title: Delete (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: c4397d91-43ef-40a9-a80e-d31501a33caa
description: Delete 要素は、ローカルクライアントストアで削除する1つのフォルダーを識別します。
ms.openlocfilehash: 68f8687b8cf0723d7fd63a3d55da8ef7c2f98f8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454982"
---
# <a name="delete-foldersync"></a>Delete (FolderSync)

**Delete**要素は、ローカルクライアントストアで削除する1つのフォルダーを識別します。 
  
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)  
- [ResponseMessages](responsemessages.md)  
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)  
- [変更 (階層)](changes-hierarchy.md)  
- [Delete (FolderSync)](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

**SyncFolderHierarchyDeleteType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |フォルダーの識別子と変更キーが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[変更 (階層)](changes-hierarchy.md) <br/> |クライアント上のフォルダーと、Microsoft Exchange Server 2007 を実行しているコンピューター上のフォルダーとの違いの種類を表す、変更の種類のシーケンス配列が含まれています。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange 2007 コンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md)
- [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

