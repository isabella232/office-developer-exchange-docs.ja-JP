---
title: SharingEffectiveRights (CalendarPermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: b519f642-a9ef-4300-92e6-ed8202855fde
description: SharingEffectiveRights 要素は、共有されている予定表データに対してユーザーが持つアクセス許可を示します。
ms.openlocfilehash: d1e669b70ad816cc24e34554a116159025e267e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547072"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a>SharingEffectiveRights (CalendarPermissionReadAccessType)

**SharingEffectiveRights** 要素は、共有されている予定表データに対してユーザーが持つアクセス許可を示します。 
  
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

次の表に **、SharingEffectiveRights 要素で使用できる値を示** します。 
  
|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |ユーザーに予定表内のアイテムを表示するアクセス許可が付与されていないかどうかを示します。  <br/> |
|TimeOnly  <br/> |ユーザーが予定表の空き時間のみ表示するアクセス許可を持っているかどうかを示します。  <br/> |
|TimeAndSubjectAndLocation  <br/> |ユーザーが予定表の空き時間情報と予定の件名と場所を表示するアクセス許可を持っているかどうかを示します。  <br/> |
|FullDetails  <br/> |ユーザーが予定表内のすべてのアイテム (空き時間と件名、場所、予定の詳細など) を表示する権限を持っているかどうかを示します。  <br/> |
   
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



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

