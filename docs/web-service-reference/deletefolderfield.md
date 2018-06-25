---
title: DeleteFolderField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderField
api_type:
- schema
ms.assetid: f9c2187b-4c60-4358-b4b4-ede50eadae48
description: DeleteFolderField 要素は、UpdateFolder の呼び出し中に、フォルダーから特定のプロパティを削除する操作を表します。
ms.openlocfilehash: d0a5fb18c5f3445982a6417007ad6af9b1b365af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759976"
---
# <a name="deletefolderfield"></a>DeleteFolderField

**DeleteFolderField**要素は、UpdateFolder の呼び出し中に、フォルダーから特定のプロパティを削除する操作を表します。 
  
- [UpdateFolder](updatefolder.md) 
- [FolderChanges](folderchanges.md)  
- [FolderChange](folderchange.md)  
- [(フォルダー) の更新](updates-folder.md) 
- [DeleteFolderField](deletefolderfield.md)
  
```xml
<DeleteFolderField>
   <FieldURI/>
</DeleteFolderField>
```

 **DeleteFolderFieldType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |ディクショナリ プロパティの個々 のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |拡張 MAPI プロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[(フォルダー) の更新](updates-folder.md) <br/> |定義する要素のセットが含まれていて、このオプションを設定すると、フォルダーのプロパティへの変更を削除します。  <br/> この要素への XPath 式は、次のようにします。`/UpdateFolder/FolderChanges/FolderChange[i]/Updates` <br/> |
   
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

- 
  [UpdateFolder 操作](updatefolder-operation.md)

