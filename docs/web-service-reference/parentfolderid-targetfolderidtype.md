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
description: ParentFolderId 要素は、新しいフォルダーを作成するフォルダー、または FindConversation 操作を検索するフォルダーを指定します。
ms.openlocfilehash: 36e63266d10603c4d453a37e2b0d22e02599e516
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467803"
---
# <a name="parentfolderid-targetfolderidtype"></a>ParentFolderId (TargetFolderIdType)

**ParentFolderId**要素は、新しいフォルダーを作成するフォルダー、または[findconversation 操作](findconversation-operation.md)を検索するフォルダーを指定します。
  
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

**ParentFolderId**要素には、2つの子要素が含まれています。 子要素は、スキーマ内で相互に排他的です。 
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |新しいフォルダーを作成するフォルダーの必須の識別子と省略可能な change キー、および[Findconversation 操作](findconversation-operation.md)の検索先のフォルダーが含まれています。 この要素を使用すると、 [DistinguishedFolderId](distinguishedfolderid.md)要素の使用は除外されます。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Microsoft Exchange Server 2007 の既定のフォルダーを識別します。 この要素を使用すると、 [FolderId](folderid.md)要素の使用は除外されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateFolder](createfolder.md) <br/> |Exchange データベースにフォルダーを作成するための要求を定義します。  <br/> この要素の XPath 式を次に示します。`/CreateFolder` <br/> |
|[FindConversation](findconversation.md) <br/> |メールボックス内のスレッドを検索する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

2つの子要素は、新しいフォルダーを格納するフォルダーを定義するために使用されます。 新しいフォルダーの親フォルダーを識別するには、 [FolderId](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)のいずれかの要素を選択する必要があります。 両方の要素を同時に使用することはできません。 この要素は、フォルダーを作成するために必要です。 
  
[ParentFolderId](parentfolderid.md)要素は、既存のアイテムとフォルダーの場所を表します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- 
  [CreateFolder 操作](createfolder-operation.md)
- [FindConversation 操作](findconversation-operation.md)
- [フォルダーの作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

