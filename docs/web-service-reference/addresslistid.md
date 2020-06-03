---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: AddressListId 要素は、アドレス一覧の識別子を指定します。
ms.openlocfilehash: c33944bf6e41903a5de596628e1ce7ba9f7421e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463609"
---
# <a name="addresslistid"></a>AddressListId

**AddressListId**要素は、アドレス一覧の識別子を指定します。 
  
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
|**Id** <br/> |文字列アドレス一覧の識別子。 この属性は必須です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |フォルダーを使用する操作を対象とするフォルダーを示します。 この要素は、ターゲットフォルダー内の会話アイテムのコピー、削除、移動、および読み取り状態の設定時に存在する必要があります。  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |電子メールアイテムのコピー先フォルダーの識別子を指定します。  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |コピー操作と移動操作の宛先フォルダーを指定します。  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |電子メールアイテムの移動先フォルダーの識別子を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

