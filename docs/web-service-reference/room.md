---
title: Room
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Room
api_type:
- schema
ms.assetid: a2cde8b8-2d31-4ebf-8171-f4dfd650d079
description: Room 要素は、会議室を表します。
ms.openlocfilehash: 062b89652ba809f245c1ac3ccee1005cbf0eabbd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523539"
---
# <a name="room"></a>Room

**Room 要素** は、会議室を表します。 
  
[Rooms](rooms.md)
  
[Room](room.md)
  
```XML
<Room>
   <Id/>
</Room>
```

 **RoomType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Id (EmailAddressType)](id-emailaddresstype.md) <br/> |会議室を表す電子メール アドレスと表示名を含む識別子。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Rooms](rooms.md) <br/> |共通機能に関連付けられた会議室の一覧 (同じ建物内など) を定義します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetRooms 操作](getrooms-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

