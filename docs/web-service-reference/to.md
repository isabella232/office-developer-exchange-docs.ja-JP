---
title: へ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- To
api_type:
- schema
ms.assetid: d14e46da-14bd-4a33-a78e-8ee314d9c1d8
description: To 要素は、タイム ゾーン遷移のターゲットを指定します。 ターゲットは、タイム ゾーン期間またはタイム ゾーン移行のグループのいずれかです。
ms.openlocfilehash: 64f3f3258fd7c2bad051eabb1b33617bb056ab39
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522552"
---
# <a name="to"></a>へ

**To 要素** は、タイム ゾーン遷移のターゲットを指定します。 ターゲットは、タイム ゾーン期間またはタイム ゾーン移行のグループのいずれかです。 
  
```xml
<To Kind=""/>
```

 **TransitionTargetType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|Kind  <br/> |タイム ゾーン移行ターゲットがタイム ゾーン期間か、タイム ゾーン移行のグループかを示します。  <br/> |
   
#### <a name="kind-attribute-values"></a>Kind 属性値

|**値**|**説明**|
|:-----|:-----|
|Period  <br/> |タイム ゾーン移行ターゲットがタイム ゾーン期間を指定します。  <br/> |
|Group  <br/> |タイム ゾーン移行ターゲットがタイム ゾーンの切り替えのグループを指定します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |特定の日付と特定の時刻に発生するタイム ゾーン遷移を表します。  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |毎年同じ日に発生するタイム ゾーン遷移を表します。  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |指定した年の日に発生するタイム ゾーンの遷移を表します。  <br/> |
|[Transition](transition.md) <br/> |タイム ゾーンの切り替えを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、タイム ゾーン遷移のターゲットである [Period](period.md) または [TransitionsGroup](transitionsgroup.md) の一意の識別子を指定する文字列です。 
  
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

