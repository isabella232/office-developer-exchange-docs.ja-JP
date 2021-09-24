---
title: TransitionsGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TransitionsGroup
api_type:
- schema
ms.assetid: 19d56080-546a-4d53-929e-363d56186759
description: TransitionsGroup 要素は、タイム ゾーン遷移の配列を表します。
ms.openlocfilehash: c24eeb803ce106224bda5b410d39298cbe57a7df
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538738"
---
# <a name="transitionsgroup"></a>TransitionsGroup

**TransitionsGroup** 要素は、タイム ゾーン遷移の配列を表します。 
  
```xml
<TransitionsGroup Id="">
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</TransitionsGroup>
```

 **ArrayOfTransitionsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |遷移グループの一意の識別子を表す文字列値。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |特定の日付と特定の時刻に発生するタイム ゾーン遷移を表します。  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |毎年同じ日に発生するタイム ゾーン遷移を表します。  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |指定した年の日に発生するタイム ゾーンの遷移を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TransitionsGroups](transitionsgroups.md) <br/> |タイム ゾーン移行グループの配列を表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Microsoft Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

