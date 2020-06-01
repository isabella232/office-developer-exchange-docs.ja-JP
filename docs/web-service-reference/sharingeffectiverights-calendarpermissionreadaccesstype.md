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
description: SharingEffectiveRights 要素は、共有されている予定表データに対してユーザーが持っているアクセス許可を示します。
ms.openlocfilehash: 5581e9cc001608a124ae94e69eba836f6fd98520
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458580"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a>SharingEffectiveRights (CalendarPermissionReadAccessType)

**SharingEffectiveRights**要素は、共有されている予定表データに対してユーザーが持っているアクセス許可を示します。 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 **CalendarPermissionReadAccessType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |主に予定表アイテムを含むフォルダーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、 **SharingEffectiveRights**要素に指定できる値を示します。 
  
|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |ユーザーが予定表のアイテムを表示する権限を持っていないことを示します。  <br/> |
|TimeOnly  <br/> |ユーザーが予定表の空き時間情報のみを表示するアクセス許可を持っていることを示します。  <br/> |
|TimeAndSubjectAndLocation  <br/> |ユーザーが予定表の空き時間情報を表示するためのアクセス許可と、予定の件名と場所を表示できることを示します。  <br/> |
|FullDetails  <br/> |ユーザーが予定表のすべてのアイテムを表示するためのアクセス許可を持っていることを示します。空き時間情報、件名、場所、および予定の詳細が含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

