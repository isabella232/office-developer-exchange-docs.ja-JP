---
title: BaseFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- BaseFolderIds
api_type:
- schema
ms.assetid: bdaa6093-f960-469a-b338-0e75aaa536c6
description: BaseFolderIds 要素は、検索フォルダーの内容を決定するためにマイニングされるフォルダーのコレクションを表します。
ms.openlocfilehash: 3a108e6215c6a444117aa65c756352b9800f6948
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518947"
---
# <a name="basefolderids"></a>BaseFolderIds

**BaseFolderIds** 要素は、検索フォルダーの内容を決定するためにマイニングされるフォルダーのコレクションを表します。 
  
```xml
<BaseFolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</BaseFolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |フォルダーの識別子と変更キーを格納します。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |名前で参照できる MicrosoftExchange Server 2007 フォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SearchParameters](searchparameters.md) <br/> |検索フォルダーを定義するパラメーターを表します。  <br/> |
   
## <a name="remarks"></a>注釈

**BaseFolderIds 要素には**、少なくとも 1 つの [FolderId](folderid.md)または [DistinguishedFolderId 要素が含まれている必要](distinguishedfolderid.md)があります。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

