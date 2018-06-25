---
title: 時間 (TimeChangeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Time
api_type:
- schema
ms.assetid: be12e41e-6871-4f6b-b2d4-3dfa404f9ea1
description: 時間要素では、標準時と夏時間との間の時間が変更されたときの時間について説明します。
ms.openlocfilehash: db44ef494561b75dc55c93229cec3901f04235ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839669"
---
# <a name="time-timechangetype"></a>時間 (TimeChangeType)

**時間**要素では、標準時と夏時間との間の時間が変更されたときの時間について説明します。 
  
```xml
<Time/>
```

 **時間**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[(夏時間)](daylight.md) <br/> |日付と時刻が変更されたとき夏時間から標準時間への時間を表します。  <br/> |
|[Standard](standard.md) <br/> |日付と時刻が変更されたとき夏時間から標準時間への時間を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、標準時と夏時間との間の時間が変更されたときの時刻を表します。
  
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

