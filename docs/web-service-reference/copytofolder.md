---
title: CopyToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyToFolder
api_type:
- schema
ms.assetid: 6fd8a6b8-d813-43ff-991b-0e9e782fe00e
description: CopyToFolder 要素に項目をコピーすることができます、電子メール フォルダーの識別子を指定します。
ms.openlocfilehash: b641c23b7aed11ae85157e2ed01cfa9d61d07e0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759786"
---
# <a name="copytofolder"></a>CopyToFolder

**CopyToFolder**要素に項目をコピーすることができます、電子メール フォルダーの識別子を指定します。 
  
```XML
<CopyToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</CopyToFolder>
```

 **TargetFolderIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[フォルダー Id](folderid.md) <br/> |先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーの識別子が含まれています。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アクション](actions.md) <br/> |条件が満たされるときに、メッセージに対して実行される使用可能なアクションのセットを表します。  <br/> |
   
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
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[MoveToFolder](movetofolder.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

