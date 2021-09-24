---
title: ConferenceType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConferenceType
api_type:
- schema
ms.assetid: 6bcf6c18-2695-44b1-aabe-dadc52b2633a
description: ConferenceType 要素は、予定表アイテムで実行される会議の種類を示します。
ms.openlocfilehash: ffb25793176dfb723581074bd73739459010ed45
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523196"
---
# <a name="conferencetype"></a>ConferenceType

**ConferenceType 要素** は、予定表アイテムで実行される会議の種類を示します。 
  
```xml
<ConferenceType/>
```

 **int**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、整数値を表すテキスト値が必要です。 この要素で使用できる値は次のとおりです。
  
- 0 = NetMeeting
    
- 1 = NetShow
    
- 2 = チャット
    
## <a name="remarks"></a>注釈

**MeetingWorkspaceUrl** プロパティは、開催者の予定表アイテムに対して読み取り/書き込み可能です。 会議出席依頼と出席者の予定表アイテムの読み取り専用です。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

