---
title: MeetingWorkspaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MeetingWorkspaceUrl
api_type:
- schema
ms.assetid: 0ca942fe-8f57-4065-93ad-65790f9a04c3
description: MeetingWorkspaceUrl 要素には、予定表アイテムに含まれる会議ワークスペースの URL が含まれます。 会議ワークスペースは、会議を計画し、結果を追跡する共有 Web サイトです。
ms.openlocfilehash: c3d051d3529e9de9288c5ecaec2d601b317e2b0b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540798"
---
# <a name="meetingworkspaceurl"></a>MeetingWorkspaceUrl

**MeetingWorkspaceUrl** 要素には、予定表アイテムに含まれる会議ワークスペースの URL が含まれます。 会議ワークスペースは、会議を計画し、結果を追跡する共有 Web サイトです。 
  
```xml
<MeetingWorkspaceUrl/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議Exchangeします。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、URL を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

MeetingWorkspaceUrl プロパティは、開催者の予定表アイテムに対して読み取り/書き込み可能です。 会議出席依頼と出席者の予定表アイテムの読み取り専用です。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

