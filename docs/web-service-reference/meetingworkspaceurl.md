---
title: MeetingWorkspaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingWorkspaceUrl
api_type:
- schema
ms.assetid: 0ca942fe-8f57-4065-93ad-65790f9a04c3
description: MeetingWorkspaceUrl 要素には、予定表アイテムに含まれている会議ワークスペースの URL が含まれています。 会議ワークスペースは、会議を計画し、結果を追跡するための共有の Web サイトです。
ms.openlocfilehash: cd4396e590ab1471278bd44b9a4e0009fe326eaf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466284"
---
# <a name="meetingworkspaceurl"></a>MeetingWorkspaceUrl

**MeetingWorkspaceUrl**要素には、予定表アイテムに含まれている会議ワークスペースの URL が含まれています。 会議ワークスペースは、会議を計画し、結果を追跡するための共有の Web サイトです。 
  
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
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、URL を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

MeetingWorkspaceUrl プロパティは、開催者の予定表アイテムの読み取り/書き込みが可能です。 会議出席依頼と出席者の予定表アイテムに対しては読み取り専用になります。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

