---
title: ArchiveSourceFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5b6a099-3b87-44ef-a197-8198730ff72d
description: ArchiveSourceFolderId 要素は、アーカイブのアイテムの元のフォルダーの Id を指定します。
ms.openlocfilehash: b7a5097de734777a71559703ed2d54199edd952e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759436"
---
# <a name="archivesourcefolderid"></a>ArchiveSourceFolderId

**ArchiveSourceFolderId**要素は、アーカイブのアイテムの元のフォルダーの Id を指定します。 
  
```XML
<ArchiveSourceFolderId>
   <FolderId/>
   <DistinguishedFolderId/>
   <AddressListId/>
</ArchiveSourceFolderId>
```

 **TargetFolderIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[フォルダー Id](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md) | [AddressListId](addresslistid.md)
  
### <a name="parent-elements"></a>親要素

[ArchiveItem](archiveitem.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

