---
title: Updates (Folder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Updates
api_type:
- schema
ms.assetid: b047e3a4-a5ab-4098-b7a0-273bc809e702
description: Updates 要素には、フォルダー のプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。
ms.openlocfilehash: cb40f2a5b66f407b02c636c5115bcab5d382a6fd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510765"
---
# <a name="updates-folder"></a>Updates (Folder)

**Updates 要素には**、フォルダー のプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。 
  
- [UpdateFolder](updatefolder.md)
  
- [FolderChanges](folderchanges.md)
  
- [FolderChange](folderchange.md)
  
- [Updates (Folder)](updates-folder.md)
  
```xml
<Updates>
   <AppendToFolderField/>
   <SetFolderField/>
   <DeleteFolderField/>
</Updates>
```

**NonEmptyArrayOfFolderChangeDescriptionsType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |UpdateFolder 操作中にフォルダー プロパティに追加する [データを表します](updatefolder-operation.md)。  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |UpdateFolder 操作のフォルダー上の 1 つのプロパティへの更新 [を表します](updatefolder-operation.md)。  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |UpdateFolder 操作中にフォルダーから特定のプロパティを削除する操作 [を表します](updatefolder-operation.md)。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderChange](folderchange.md) <br/> |1 つのフォルダーに対して実行する変更のコレクションを表します。  <br/> 次に、この要素の XPath 式を示します。  `/UpdateFolder/FolderChanges/FolderChange[i]` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [UpdateFolder 操作](updatefolder-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

