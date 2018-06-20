---
title: SharingEffectiveRights (CalendarPermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: b519f642-a9ef-4300-92e6-ed8202855fde
description: SharingEffectiveRights 要素は、ユーザーが共有されている予定表データを持っているアクセス許可を示します。
ms.openlocfilehash: e7d2aa061650c33d27de042ae8a6348f9a7d3430
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833480"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a>SharingEffectiveRights (CalendarPermissionReadAccessType)

**SharingEffectiveRights**要素は、ユーザーが共有されている予定表データを持っているアクセス許可を示します。 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 **CalendarPermissionReadAccessType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |主に予定表のアイテムを含むフォルダーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表は、 **SharingEffectiveRights**要素の値を一覧します。 
  
|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |ユーザーに予定表にアイテムを表示する権限がないことを示します。  <br/> |
|TimeOnly  <br/> |ユーザーが予定表の空き時間のみを表示する権限を持っていることを示します。  <br/> |
|TimeAndSubjectAndLocation  <br/> |ユーザーが予定表、件名、予定の場所に空き時間情報を表示するアクセス許可を持っていることを示します。  <br/> |
|FullDetails  <br/> |ユーザーが空き時間情報、件名、場所、および予定の詳細情報を含む、予定表のすべての項目を表示する権限を持っていることを示します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

