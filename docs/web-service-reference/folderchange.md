---
title: FolderChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderChange
api_type:
- schema
ms.assetid: 23279750-131b-4e1a-b7d1-be235c4e0891
description: FolderChange 要素は、1つのフォルダーに対して実行される変更のコレクションを表します。
ms.openlocfilehash: e4a025bef100fdd478be545b6448b15886e47c60
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530240"
---
# <a name="folderchange"></a>FolderChange

**Folderchange**要素は、1つのフォルダーに対して実行される変更のコレクションを表します。 
  
- [UpdateFolder](updatefolder.md) 
- [FolderChanges 変更](folderchanges.md) 
- [FolderChange](folderchange.md)
  
```xml
<FolderChange>
   <FolderId/>
   <Updates/>
</FolderChange>
```

```xml
<FolderChange>
   <DistinguishedFolderId/>
   <Updates/>
</FolderChange>
```

**FolderChangeType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |更新するフォルダーの識別子と変更キーが含まれています。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |名前で参照できる Microsoft Exchange Server 2007 フォルダーを識別します。  <br/> |
|[Updates (フォルダー)](updates-folder.md) <br/> |[FolderId](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)のいずれかの要素によって識別されるフォルダーに対して実行される更新の種類を定義します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderChanges 変更](folderchanges.md) <br/> |フォルダーに対する変更のコレクションを表します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [UpdateFolder 操作](updatefolder-operation.md)

