---
title: GetRooms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRooms
api_type:
- schema
ms.assetid: 82a737c7-da41-4777-8ad8-89851a0b602b
description: GetRooms 要素は、特定の会議室の一覧内の会議室の一覧を取得する要求のルート要素です。
ms.openlocfilehash: a787097752cfeee9489e5f118549c2d939ba4c9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760851"
---
# <a name="getrooms"></a>GetRooms

**GetRooms**要素は、特定の会議室の一覧内の会議室の一覧を取得する要求のルート要素です。 
  
```XML
<GetRooms>
   <RoomList/>
</GetRooms>
```

 **GetRoomsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[RoomList](roomlist.md) <br/> |会議室の一覧を識別する電子メール アドレスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
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
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

