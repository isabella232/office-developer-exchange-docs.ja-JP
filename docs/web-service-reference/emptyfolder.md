---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: EmptyFolder 要素は、Exchange ストア内のメールボックス内のフォルダーを空にする要求を定義します。 必要に応じて、フォルダーを空にしたときにサブフォルダーを削除することもできます。
ms.openlocfilehash: a42e4e3f25741a96ee65fe6f87fc3236b68f4dc9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457278"
---
# <a name="emptyfolder"></a>EmptyFolder

**Emptyfolder**要素は、Exchange ストア内のメールボックス内のフォルダーを空にする要求を定義します。 必要に応じて、フォルダーを空にしたときにサブフォルダーを削除することもできます。 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 **EmptyFolderType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**DeleteType** <br/> |フォルダーを空にする方法を指定します。 この属性は必須です。  <br/> |
|**DeleteSubFolders** <br/> |サブフォルダーを削除するかどうかを指定します。 この属性は必須です。  <br/> |
   
#### <a name="deletetype-attribute"></a>DeleteType 属性

|**値**|**説明**|
|:-----|:-----|
|HardDelete  <br/> |メッセージとフォルダーがストアから完全に削除されます。  <br/> |
|SoftDelete  <br/> |収集が有効になっている場合、メッセージとフォルダーは収集に移動されます。  <br/> |
|MoveToDeletedItems  <br/> |メッセージとフォルダーが [削除済みアイテム] フォルダーに移動されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |削除するフォルダーを識別するために使用されるフォルダー識別子の配列を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[EmptyFolder 操作](emptyfolder-operation.md)

