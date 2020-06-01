---
title: Nonindexableitemの取得結果
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7cbdbc21-5405-4cbc-8ca0-d7b0257927aa
description: Nonindexableitem詳細 Result 要素は、GetNonIndexableItemDetails WSDL 操作の結果を指定します。
ms.openlocfilehash: 647f58b5e7285af70bbfb3a203ba71c9a3ccebcc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465444"
---
# <a name="nonindexableitemdetailsresult"></a>Nonindexableitemの取得結果

**Nonindexableitem詳細 result**要素は、 **getnonindexableitemdetails** WSDL 操作の結果を指定します。 
  
```XML
<NonIndexableItemDetailsResult>
   <Items/>
   <FailedMailboxes/>
</NonIndexableItemDetailsResult>
```

 **Nonindexableitemの Resulttype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[アイテム (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) 、[失敗したメールボックス](failedmailboxes.md)
  
### <a name="parent-elements"></a>親要素

[GetnonindexableitemGetNonIndexableItemDetailsResponseMessage の応答](getnonindexableitemdetailsresponse.md)、 [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetNonIndexableItemDetails 操作](getnonindexableitemdetails-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

