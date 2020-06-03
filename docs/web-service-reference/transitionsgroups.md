---
title: 遷移のグループ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TransitionsGroups
api_type:
- schema
ms.assetid: ad0849f8-5158-4a23-9c36-a49f5be1d1e1
description: 推移 Tionsgroups 要素は、タイムゾーン遷移グループの配列を表します。
ms.openlocfilehash: 35244e122ee31045359afd0833459bbb94fd0aa1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467411"
---
# <a name="transitionsgroups"></a>遷移のグループ

**推移 Tionsgroups**要素は、タイムゾーン遷移グループの配列を表します。 
  
```XML
<TransitionsGroups>
   <TransitionsGroup/>
</TransitionsGroups>
```

 **Arrayof遷移 Tionsgroupstype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[遷移 Tionsgroup](transitionsgroup.md) <br/> |タイムゾーンの切り替えの配列を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StartTimeZone](starttimezone.md) <br/> |[Calendaritem](calendaritem.md)または[会議要求](meetingrequest.md)の開始時刻のタイムゾーンを定義します。  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |[Calendaritem](calendaritem.md)または[会議の要求](meetingrequest.md)の終了時刻のタイムゾーンを定義します。  <br/> |
|[TimeZoneDefinition](timezonedefinition.md) <br/> |タイムゾーンを定義します。  <br/> |
   
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

