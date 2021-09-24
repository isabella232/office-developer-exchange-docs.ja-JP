---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: ToFolderId 要素は、コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを表します。
ms.openlocfilehash: b58192aa4d1ffe609da78dfdf1b5c86522fc45c8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515167"
---
# <a name="tofolderid"></a>ToFolderId

**ToFolderId 要素は**、コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを表します。 
  
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
|[FolderId](folderid.md) <br/> |コピーまたは移動したアイテムまたはフォルダーの移動先フォルダーの識別子を格納します。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |コピーまたは移動されたアイテムまたはフォルダーの名前付き移動先フォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MoveFolder](movefolder.md) <br/> |フォルダーストア内のフォルダーを移動する要求Exchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |フォルダー ストア内のフォルダーをコピーする要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/CopyFolder` <br/> |
|[MoveItem](moveitem.md) <br/> |ストア内のアイテムを移動する要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |アイテム ストア内のアイテムをコピーする要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [MoveFolder 操作](movefolder-operation.md)  
- [CopyFolder 操作](copyfolder-operation.md) 
- [MoveItem 操作](moveitem-operation.md) 
- [CopyItem 操作](copyitem-operation.md)

