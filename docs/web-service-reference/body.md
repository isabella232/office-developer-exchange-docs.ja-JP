---
title: 本文
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7851ea9b-9f87-4adc-a26f-7a27df4a9bca
description: Body 要素は、アイテムの本文を指定します。
ms.openlocfilehash: 47f0726c6ef329fbbefc99be3b1e2d605f852afa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526849"
---
# <a name="body"></a>Body

**Body 要素** は、アイテムの本文を指定します。 
  
```XML
<Body> BodyType="" IsTruncated="" </Body>
```

 **BodyType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|BodyType  <br/> |本文の種類を指定します。  <br/> |
|IsTruncated  <br/> |本文が切り捨てられるかどうかを示すブール値。  <br/> |
   
#### <a name="bodytype"></a>BodyType

|**値**|**説明**|
|:-----|:-----|
|HTML  <br/> |本文が HTML 内にあるかどうかを示します。  <br/> |
|テキスト  <br/> |本文がテキスト内にあるかどうかを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[Contact](contact.md) <br/> |ストア内の連絡先アイテムExchangeします。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[項目](item.md) <br/> |ストア内の汎用アイテムをExchangeします。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Microsoft の電子メール Exchangeを表します。  <br/> |
|[PostItem](postitem.md) <br/> |ストア内の投稿アイテムをExchangeします。  <br/> |
|[タスク](task.md) <br/> |ストア内のタスクをExchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

Body 要素のテキスト **値** は、アイテムの本文コンテンツです。 
  
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

