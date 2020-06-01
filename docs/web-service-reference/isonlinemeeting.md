---
title: IsOnlineMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsOnlineMeeting
api_type:
- schema
ms.assetid: c29df676-0f3a-4694-a42f-522c6d16872f
description: IsOnlineMeeting 要素は、会議がオンラインかどうかを示します。
ms.openlocfilehash: d2d60c8a51ad7e03c33b57709d9173e79d162268
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460401"
---
# <a name="isonlinemeeting"></a>IsOnlineMeeting

**IsOnlineMeeting**要素は、会議がオンラインかどうかを示します。 
  
```xml
<IsOnlineMeeting/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、ブール値を表すテキスト値が必要です。 値が**true の場合**は、会議がオンラインであることを示します。 値が**false**の場合は、会議がオンラインになっていないことを示します。 
  
## <a name="remarks"></a>注釈

IsOnlineMeeting プロパティは、開催者の予定表アイテムの読み取り/書き込みが可能です。 会議出席依頼と出席者の予定表アイテムに対しては読み取り専用になります。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

