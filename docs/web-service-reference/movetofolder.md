---
title: MoveToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveToFolder
api_type:
- schema
ms.assetid: 991673b9-b627-4848-bfba-59a187b8575f
description: MoveToFolder 要素は、電子メール アイテムの移動先となるフォルダーの識別子を指定します。
ms.openlocfilehash: 058f008b348d49c932bf334dd3379f02d06154e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832494"
---
# <a name="movetofolder"></a>MoveToFolder

**MoveToFolder**要素は、電子メール アイテムの移動先となるフォルダーの識別子を指定します。 
  
```XML
<MoveToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</MoveToFolder>
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



[CopyToFolder](copytofolder.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

