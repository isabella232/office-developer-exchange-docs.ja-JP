---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: ToFolderId 要素は、先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーを表します。
ms.openlocfilehash: 9d2fd6c177711cfe3a5d3415320440259e2f5289
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353659"
---
# <a name="tofolderid"></a>ToFolderId

**ToFolderId**要素は、先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーを表します。 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

```xml
<ToFolderId>
   <DistinguishedFolderId/>
</ToFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーの識別子が含まれています。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MoveFolder](movefolder.md) <br/> |Exchange ストア内のフォルダーを移動する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Exchange ストア内のフォルダーをコピーするのには要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/CopyFolder` <br/> |
|[MoveItem](moveitem.md) <br/> |Exchange ストア内のアイテムを移動する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Exchange ストア内の項目をコピーするための要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>注釈

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [MoveFolder 操作](movefolder-operation.md)  
- [CopyFolder 操作](copyfolder-operation.md) 
- 
  [MoveItem 操作](moveitem-operation.md) 
- 
  [CopyItem 操作](copyitem-operation.md)

