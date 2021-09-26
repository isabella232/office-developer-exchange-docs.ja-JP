---
title: ReferenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ReferenceItemId
api_type:
- schema
ms.assetid: 8fd4bb12-a94b-43f5-be3b-f435684e311d
description: ReferenceItemId 要素は、応答オブジェクトが参照するアイテムを識別します。
ms.openlocfilehash: b6ddb59eb3f266aff6400429ac8178f5640bf06b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542860"
---
# <a name="referenceitemid"></a>ReferenceItemId

**ReferenceItemId 要素** は、応答オブジェクトが参照するアイテムを識別します。 
  
```xml
<ReferenceItemId Id="" ChangeKey="" />
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |ストア内の特定のアイテムExchangeします。  <br/> |
|**ChangeKey** <br/> |アイテムの特定のバージョンを識別します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼に対する Accept 返信を表します。  <br/> |
|[AcceptSharingInvitation](acceptsharinginvitation.md) <br/> |共有の招待に対する Accept 返信を表します。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議のキャンセルに使用される応答オブジェクトを表します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼に対する辞退の返信を表します。  <br/> |
|[ForwardItem](forwarditem.md) <br/> |受信者に転送Exchangeストア アイテムを格納します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |アイテムをストアからExchangeします。  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |アイテムストア内のアイテムの識別された受信者全員に対する返信Exchangeします。  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |ストア内のアイテムの作成者への返信Exchangeします。  <br/> |
|[SuppressReadReceipt](suppressreadreceipt.md) <br/> |読み取り受信要求に応答するために使用します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に対する仮返信を表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

