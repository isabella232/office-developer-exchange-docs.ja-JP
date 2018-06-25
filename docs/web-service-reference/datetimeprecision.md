---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: DateTimePrecision 要素は、返される日付と時刻の値の有効桁数を指定します。
ms.openlocfilehash: 4d11598628228b41adf021adbbaa77e6348534bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759918"
---
# <a name="datetimeprecision"></a>DateTimePrecision

**DateTimePrecision**要素は、返される日付と時刻の値の有効桁数を指定します。 
  
```XML
<DateTimePrecision />
```

**DateTimePrecisionType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

**DateTimePrecision**要素は、SOAP ヘッダーに配置されます。 
  
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 指定可能な値は次のいずれかです。
  
- 秒
    
- (ミリ秒)
    
## <a name="remarks"></a>備考

「秒」に設定する**DateTimePrecision**要素を使用して SOAP ヘッダーを使用すると日付/時刻値が最も近い秒に返されます (00: 00:00)。 「ミリ秒」を使用する場合の日付と時刻に最も近いミリ秒 (00:00:00.0000) の値が返されます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

