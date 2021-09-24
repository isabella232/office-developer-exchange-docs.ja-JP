---
title: Ids
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Ids
api_type:
- schema
ms.assetid: c54cdeaf-6761-4d1a-a329-fb279f0e2a64
description: Ids 要素には、タイム ゾーン定義識別子の配列が含まれる。
ms.openlocfilehash: a5ff1899a50b13213e07005210609194ece61542
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529792"
---
# <a name="ids"></a>Ids

**Ids 要素には**、タイム ゾーン定義識別子の配列が含まれる。 
  
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
|[Id (TimeZone)](id-timezone.md) <br/> |1 つのタイム ゾーン定義を識別する要素。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetServerTimeZones](getservertimezones.md) <br/> |サーバーからタイム ゾーン定義を取得する要求をExchangeします。  <br/> |
   
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

