---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: EmptyFolder 要素は、Exchange ストア内のメールボックス内のフォルダーを空にする要求を定義します。 オプションでは、サブフォルダーは、フォルダーを空にしたときにも削除できます。
ms.openlocfilehash: c72e11cea29e2e55c9c29754eec60e73bd1e4d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760269"
---
# <a name="emptyfolder"></a>EmptyFolder

**EmptyFolder**要素は、Exchange ストア内のメールボックス内のフォルダーを空にする要求を定義します。 オプションでは、サブフォルダーは、フォルダーを空にしたときにも削除できます。 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 **EmptyFolderType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**削除の種類** <br/> |フォルダーを空にする方法を指定します。 この属性は、必要があります。  <br/> |
|**DeleteSubFolders** <br/> |サブフォルダーを削除するかどうかを指定します。 この属性は、必要があります。  <br/> |
   
#### <a name="deletetype-attribute"></a>削除の種類の属性

|**値**|**説明**|
|:-----|:-----|
|HardDelete  <br/> |A メッセージおよびフォルダーがストアから完全に削除します。  <br/> |
|SoftDelete  <br/> |A メッセージおよびフォルダーを移動する、ごみ箱をあさる場合、収集を有効にします。  <br/> |
|MoveToDeletedItems  <br/> |A のメッセージとフォルダーは削除済みアイテム フォルダーに移動します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |削除するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[EmptyFolder 操作](emptyfolder-operation.md)

