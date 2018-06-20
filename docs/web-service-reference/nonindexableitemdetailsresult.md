---
title: NonIndexableItemDetailsResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7cbdbc21-5405-4cbc-8ca0-d7b0257927aa
description: NonIndexableItemDetailsResult 要素は、GetNonIndexableItemDetails の WSDL 操作の結果を指定します。
ms.openlocfilehash: 6e271f2cf0e37f26b945332c94167b6a42354115
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832535"
---
# <a name="nonindexableitemdetailsresult"></a>NonIndexableItemDetailsResult

**NonIndexableItemDetailsResult**要素は、 **GetNonIndexableItemDetails**の WSDL 操作の結果を指定します。 
  
```XML
<NonIndexableItemDetailsResult>
   <Items/>
   <FailedMailboxes/>
</NonIndexableItemDetailsResult>
```

 **NonIndexableItemDetailResultType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[アイテム (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) 、 [FailedMailboxes](failedmailboxes.md)
  
### <a name="parent-elements"></a>親要素

[GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md) 、 [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetNonIndexableItemDetails 操作](getnonindexableitemdetails-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

