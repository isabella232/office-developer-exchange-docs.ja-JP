---
title: ParentFolderId (TargetFolderIdType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 0e3e6e5f-06d0-499b-8ca4-d36036521658
description: ParentFolderId 要素内のフォルダーを識別する新しいフォルダーを作成するか、FindConversation の操作を検索するフォルダーです。
ms.openlocfilehash: 61072e1dd3321beb5f3b76d9accf20530b443796
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832686"
---
# <a name="parentfolderid-targetfolderidtype"></a>ParentFolderId (TargetFolderIdType)

**ParentFolderId**要素内のフォルダーを識別する新しいフォルダーを作成または[操作の FindConversation](findconversation-operation.md)を検索するフォルダーです。
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>属性および要素

**ParentFolderId**要素には、2 つの子要素が含まれています。 子要素は、スキーマ内で相互に排他的です。 
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[フォルダー Id](folderid.md) <br/> |必須の識別子とキーを含む、省略可能な変更でフォルダーの新しいフォルダーを作成または[FindConversation 操作](findconversation-operation.md)のために検索されるフォルダーです。 この要素を使用するには、 [DistinguishedFolderId](distinguishedfolderid.md)要素の使用が含まれません。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Microsoft Exchange Server 2007 の既定のフォルダーを識別します。 この要素を使用して、[フォルダー Id](folderid.md)要素の使用が除外されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateFolder](createfolder.md) <br/> |Exchange データベース内のフォルダーを作成する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。`/CreateFolder` <br/> |
|[FindConversation](findconversation.md) <br/> |メールボックス内の会話を検索するための要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

2 つの子要素を使用して、新しいフォルダーを格納するフォルダーを定義します。 [フォルダー Id](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)要素のいずれか、新しいフォルダーの親フォルダーを識別するを選択する必要があります。 同時に両方の要素を使用することはできません。 この要素は、フォルダーを作成する必要があります。 
  
[ParentFolderId](parentfolderid.md)要素では、既存のアイテムとフォルダーの場所について説明します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- 
  [CreateFolder 操作](createfolder-operation.md)
- 
  [FindConversation 操作](findconversation-operation.md)
- [フォルダー (Exchange Web サービス) を作成します。](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

