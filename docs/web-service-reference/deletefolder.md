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
description: DeleteFolder 要素は、Exchange ストア内のメールボックスからフォルダーを削除する要求を定義します。
ms.openlocfilehash: d31f98f26f537104e40b303de4199f45c65f49c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759978"
---
# <a name="deletefolder"></a>DeleteFolder

**DeleteFolder**要素は、Exchange ストア内のメールボックスからフォルダーを削除する要求を定義します。 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 **DeleteFolderType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**削除の種類** <br/> |フォルダーを削除する方法について説明します。 この属性は、必要があります。  <br/> |
   
#### <a name="deletetype-attribute"></a>削除の種類の属性

|**値**|**説明**|
|:-----|:-----|
|HardDelete  <br/> |フォルダーはストアから完全に削除されます。  <br/> |
|SoftDelete  <br/> |フォルダーを移動、ごみ箱をあさる場合、収集を有効にします。  <br/> |
|MoveToDeletedItems  <br/> |フォルダーは、削除済みアイテム フォルダーに移動されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |削除するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

**MoveToDeletedItems**および**HardDelete**オプションは、時間によって、Web サービスの呼び出しが完了していることを意味する、トランザクション、データベースは削除済みアイテム フォルダーにアイテムを移動または Exchange データベースから項目を完全に削除します。 この現象は、MicrosoftExchange Server 2007 および Exchange Server 2010 と同じです。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [DeleteFolder 操作](deletefolder-operation.md)

