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
description: BaseFolderIds 要素は、検索フォルダーの内容を判断するためにマイニングするフォルダーのコレクションを表します。
ms.openlocfilehash: 960e4d9c1d6eb37bf988bf163e696cbba3e1ef6f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759482"
---
# <a name="basefolderids"></a>BaseFolderIds

**BaseFolderIds**要素は、検索フォルダーの内容を判断するためにマイニングするフォルダーのコレクションを表します。 
  
```xml
<BaseFolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</BaseFolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[フォルダー Id](folderid.md) <br/> |フォルダーの識別子と変更キーが含まれています。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |名前で参照することができます MicrosoftExchange Server 2007 フォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SearchParameters](searchparameters.md) <br/> |検索フォルダーを定義するパラメーターを表します。  <br/> |
   
## <a name="remarks"></a>備考

**BaseFolderIds**要素は、少なくとも 1 つの[フォルダー Id](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)の要素を含める必要があります。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

