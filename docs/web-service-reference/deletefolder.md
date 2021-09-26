---
title: DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: e37963f4-af9e-4481-b389-16175711e66d
description: DeleteFolder 要素は、メールボックス ストア内のメールボックスからフォルダーを削除する要求Exchangeします。
ms.openlocfilehash: d1d64b84604acec54d9153144e5bfd7abaece94c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542478"
---
# <a name="deletefolder"></a>DeleteFolder

**DeleteFolder 要素は**、メールボックス ストア内のメールボックスからフォルダーを削除する要求Exchangeします。 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 **DeleteFolderType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**DeleteType** <br/> |フォルダーを削除する方法について説明します。 この属性は必須です。  <br/> |
   
#### <a name="deletetype-attribute"></a>DeleteType 属性

|**値**|**説明**|
|:-----|:-----|
|HardDelete  <br/> |フォルダーはストアから完全に削除されます。  <br/> |
|SoftDelete  <br/> |ゴミ箱が有効になっている場合、フォルダーはゴミ箱に移動されます。  <br/> |
|MoveToDeletedItems  <br/> |フォルダーが [削除済みアイテム] フォルダーに移動されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |削除するフォルダーを識別するために使用されるフォルダー識別子の配列を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

**MoveToDeletedItems** および **HardDelete** オプションはトランザクションであり、Web サービス呼び出しが完了すると、データベースはアイテムを削除済みアイテム フォルダーに移動するか、Exchange データベースからアイテムを完全に削除しました。 この動作は、MicrosoftExchange Server 2007 および 2010 Exchange Serverです。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [DeleteFolder 操作 ](deletefolder-operation.md)

