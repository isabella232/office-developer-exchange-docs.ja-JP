---
title: BaseFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseFolderIds
api_type:
- schema
ms.assetid: bdaa6093-f960-469a-b338-0e75aaa536c6
description: BaseFolderIds 要素は、検索フォルダーの内容を確認するためにマイニングされるフォルダーのコレクションを表します。
ms.openlocfilehash: 97159ec1ded685e63aafedfaf90a06eff39adaab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460268"
---
# <a name="basefolderids"></a>BaseFolderIds

**BaseFolderIds**要素は、検索フォルダーの内容を確認するためにマイニングされるフォルダーのコレクションを表します。 
  
```xml
<BaseFolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</BaseFolderIds>
```

 **非 Emptyarrayofbasefolderidstype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |フォルダーの識別子と変更キーが含まれています。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |名前で参照できる Microsoft Exchange Server 2007 フォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SearchParameters](searchparameters.md) <br/> |検索フォルダーを定義するパラメーターを表します。  <br/> |
   
## <a name="remarks"></a>注釈

**BaseFolderIds**要素には、少なくとも1つの[FolderId](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)要素が含まれている必要があります。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

