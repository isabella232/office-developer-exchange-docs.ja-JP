---
title: Updates (フォルダー)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: b047e3a4-a5ab-4098-b7a0-273bc809e702
description: Updates 要素には、フォルダーのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。
ms.openlocfilehash: 3282171dfc188a9d4735a19a97e80fe0e2f79b89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457180"
---
# <a name="updates-folder"></a>Updates (フォルダー)

**Updates**要素には、フォルダーのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。 
  
- [UpdateFolder](updatefolder.md)
  
- [FolderChanges 変更](folderchanges.md)
  
- [FolderChange](folderchange.md)
  
- [Updates (フォルダー)](updates-folder.md)
  
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
|[AppendToFolderField](appendtofolderfield.md) <br/> |[Updatefolder 操作](updatefolder-operation.md)中に folder プロパティに追加するデータを表します。  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |[Updatefolder 操作](updatefolder-operation.md)のフォルダーの1つのプロパティに対する更新を表します。  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |[Updatefolder 操作](updatefolder-operation.md)中にフォルダーから特定のプロパティを削除する操作を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderChange](folderchange.md) <br/> |1つのフォルダーに対して実行される変更のコレクションを表します。  <br/> この要素の XPath 式を次に示します。`/UpdateFolder/FolderChanges/FolderChange[i]` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [UpdateFolder 操作](updatefolder-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

