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
description: ToFolderId 要素は、コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを表します。
ms.openlocfilehash: c9cceb17fd55b7357d54b37bf4c8da1137d39b6a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44468776"
---
# <a name="tofolderid"></a>ToFolderId

**ToFolderId**要素は、コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを表します。 
  
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

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |コピーまたは移動したアイテムまたはフォルダーの宛先フォルダーの識別子が含まれています。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |コピーまたは移動されたアイテムまたはフォルダーについて、名前付きの移動先フォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MoveFolder](movefolder.md) <br/> |Exchange ストア内のフォルダーを移動する要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Exchange ストア内のフォルダーをコピーするための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/CopyFolder` <br/> |
|[MoveItem](moveitem.md) <br/> |Exchange ストア内のアイテムを移動する要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Exchange ストア内のアイテムをコピーするための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [MoveFolder 操作](movefolder-operation.md)  
- [CopyFolder 操作](copyfolder-operation.md) 
- [MoveItem 操作](moveitem-operation.md) 
- [CopyItem 操作](copyitem-operation.md)

