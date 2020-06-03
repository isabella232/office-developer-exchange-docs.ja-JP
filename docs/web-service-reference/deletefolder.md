---
title: DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: e37963f4-af9e-4481-b389-16175711e66d
description: DeleteFolder 要素は、Exchange ストア内のメールボックスからフォルダーを削除するための要求を定義します。
ms.openlocfilehash: eb705a47b78b19c79b2e87561ba3696ed40e09cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458769"
---
# <a name="deletefolder"></a>DeleteFolder

**Deletefolder**要素は、Exchange ストア内のメールボックスからフォルダーを削除するための要求を定義します。 
  
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
|**DeleteType** <br/> |フォルダーが削除される方法について説明します。 この属性は必須です。  <br/> |
   
#### <a name="deletetype-attribute"></a>DeleteType 属性

|**値**|**説明**|
|:-----|:-----|
|HardDelete  <br/> |フォルダーがストアから完全に削除されます。  <br/> |
|SoftDelete  <br/> |収集が有効になっている場合、フォルダーは収集に移動されます。  <br/> |
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

**MoveToDeletedItems**および**ハード削除**オプションは、トランザクションであり、Web サービスの呼び出しが完了すると、データベースがアイテムを削除済みアイテムフォルダーに移動したか、または Exchange データベースからアイテムを完全に削除したことを意味します。 この動作は、Microsoft Exchange Server 2007 および Exchange Server 2010 の場合と同じです。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [DeleteFolder 操作 ](deletefolder-operation.md)

