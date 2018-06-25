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
description: FolderChange 要素は、1 つのフォルダーで実行される変更のコレクションを表します。
ms.openlocfilehash: 3f8b42ff4ac88eaef53d1d4ec1d61212bc14b8c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760563"
---
# <a name="folderchange"></a>FolderChange

**FolderChange**要素は、1 つのフォルダーで実行される変更のコレクションを表します。 
  
[UpdateFolder](updatefolder.md)
  
[FolderChanges](folderchanges.md)
  
[FolderChange](folderchange.md)
  
```xml
<FolderChange>
   <FolderId/>
   <Updates/>
</FolderChange>
```

 **FolderChangeType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[フォルダー Id](folderid.md) <br/> |更新するフォルダーの識別子と変更キーが含まれています。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |名前で参照することができます MicrosoftExchange Server 2007 フォルダーを識別します。  <br/> |
|[(フォルダー) の更新](updates-folder.md) <br/> |[フォルダー Id](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)のいずれかの要素によって指定されているフォルダーに対して実行される更新の種類を定義します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderChanges](folderchanges.md) <br/> |フォルダーの変更のコレクションを表します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [UpdateFolder 操作](updatefolder-operation.md)

