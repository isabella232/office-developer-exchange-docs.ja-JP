---
title: ParentFolderId (TargetFolderIdType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 0e3e6e5f-06d0-499b-8ca4-d36036521658
description: ParentFolderId 要素は、新しいフォルダーが作成されるフォルダー、または FindConversation 操作を検索するフォルダーを識別します。
ms.openlocfilehash: 53a5721b2c20c211a61b7e71b2e4f636700456b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524624"
---
# <a name="parentfolderid-targetfolderidtype"></a>ParentFolderId (TargetFolderIdType)

**ParentFolderId** 要素は、新しいフォルダーが作成されるフォルダー、[または FindConversation](findconversation-operation.md)操作を検索するフォルダーを識別します。
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

```xml
<ParentFolderId>
   <FolderId/> 
</ParentFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>属性と要素

**ParentFolderId 要素には**、2 つの子要素が含まれています。 子要素は、スキーマ内で相互に排他的です。 
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |新しいフォルダーが作成されるフォルダー、または [FindConversation](findconversation-operation.md)操作を検索するフォルダーの必要な識別子とオプションの変更キーが含まれる。 この要素を使用すると [、DistinguishedFolderId 要素の使用が除外](distinguishedfolderid.md) されます。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |2007 フォルダー Microsoft Exchange Server既定のフォルダーを識別します。 この要素を使用すると [、FolderId 要素の使用は除外](folderid.md) されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateFolder](createfolder.md) <br/> |データベースにフォルダーを作成する要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  `/CreateFolder` <br/> |
|[FindConversation](findconversation.md) <br/> |メールボックス内の会話を検索する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

2 つの子要素を使用して、新しいフォルダーを含むフォルダーを定義します。 新しいフォルダーの親 [フォルダーを識別するには、FolderId](folderid.md) または [DistinguishedFolderId](distinguishedfolderid.md) 要素のいずれかを選択する必要があります。 両方の要素を同時に使用することはできません。 フォルダーを作成するには、この要素が必要です。 
  
[ParentFolderId 要素](parentfolderid.md)は、既存のアイテムとフォルダーの場所を表します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [CreateFolder 操作](createfolder-operation.md)
- [FindConversation 操作](findconversation-operation.md)
- [フォルダーの作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

