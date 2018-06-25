---
title: CopyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: 7d5cd08a-fe81-4cb6-a5a0-6dec2d3c93d4
description: CopyFolder 要素は、Exchange ストア内のメールボックスでフォルダーをコピーするための要求を定義します。
ms.openlocfilehash: 7bcfcc7f4212b3a3bd339fa5863df2990eb20d6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759780"
---
# <a name="copyfolder"></a>CopyFolder

**CopyFolder**要素は、Exchange ストア内のメールボックスでフォルダーをコピーするための要求を定義します。 
  
```xml
<CopyFolder>
   <ToFolderId/>
   <FolderIds/>
</CopyFolder>
```

 **CopyFolderType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ToFolderId](tofolderid.md) <br/> |コピーしたフォルダーのコピー先フォルダーを表します。  <br/> |
|[FolderIds](folderids.md) <br/> |[ToFolderId](tofolderid.md)要素で指定されたフォルダーにコピーするフォルダーの配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[CopyFolder 操作](copyfolder-operation.md)

