---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: AddressListId 要素は、アドレス一覧の識別子を指定します。
ms.openlocfilehash: 5348c6877e24fcc0c8873df1098f8a8e30fe4c1c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541561"
---
# <a name="addresslistid"></a>AddressListId

**AddressListId 要素** は、アドレス一覧の識別子を指定します。 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 **AddressListIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |文字列アドレス一覧識別子。 この属性は必須です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |フォルダーを使用するアクションの対象となるフォルダーを示します。 この要素は、ターゲット フォルダー内の会話アイテムの読み取り状態をコピー、削除、移動、および設定するときに存在する必要があります。  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |電子メール アイテムがコピーされるフォルダーの識別子を指定します。  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |コピーおよび移動アクションの移動先フォルダーを示します。  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |電子メール アイテムを移動するフォルダーの識別子を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

