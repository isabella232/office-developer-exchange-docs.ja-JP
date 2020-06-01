---
title: GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce3994c1-3bb4-4571-b026-34a6c5705410
description: GetNonIndexableItemDetails 要素は、インデックス付けされていないアイテムの詳細を取得するための要求を指定します。
ms.openlocfilehash: 1c04b4cd7a86183210be869973c9779188fa0adf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458601"
---
# <a name="getnonindexableitemdetails"></a>GetNonIndexableItemDetails

**Getnonindexableitemdetails**要素は、インデックス付けされていないアイテムの詳細を取得するための要求を指定します。 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 **GetNonIndexableItemDetailsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[メールボックス (NonEmptyArrayOfLegacyDNsType)](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |**メールボックス**要素の配列を指定します。  <br/> |
|[PageSize](pagesize.md) <br/> |検索結果に対して単一のページで返されるアイテムの数を格納します。  <br/> |
|[PageItemReference](pageitemreference.md) <br/> |ページアイテムの参照を指定します。  <br/> |
|[ページの方向](pagedirection.md) <br/> |検索結果の改ページ位置の方向を含みます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

