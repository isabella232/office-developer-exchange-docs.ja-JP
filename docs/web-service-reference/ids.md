---
title: Rid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Ids
api_type:
- schema
ms.assetid: c54cdeaf-6761-4d1a-a329-fb279f0e2a64
description: Ids 要素には、タイムゾーン定義識別子の配列が含まれています。
ms.openlocfilehash: 1c5a6974c8d3abc318ff122f3db09d8c3472dc65
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457621"
---
# <a name="ids"></a>Rid

**Ids**要素には、タイムゾーン定義識別子の配列が含まれています。 
  
```XML
<Ids>
   <Id/>
</Ids>
```

 **NonEmptyArrayOfTimeZoneIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Id (TimeZone)](id-timezone.md) <br/> |1つのタイムゾーン定義を識別する要素。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetServerTimeZones](getservertimezones.md) <br/> |Exchange サーバーからタイムゾーン定義を取得するための要求を定義します。  <br/> |
   
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

