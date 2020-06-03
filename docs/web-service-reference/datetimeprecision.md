---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: DateTimePrecision 要素は、返される日付/時刻の値の精度を指定します。
ms.openlocfilehash: 9d245dfb0123daae42ba9b9b4e98aff872b67d80
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529225"
---
# <a name="datetimeprecision"></a>DateTimePrecision

**DateTimePrecision**要素は、返される日付/時刻の値の精度を指定します。 
  
```XML
<DateTimePrecision />
```

**DateTimePrecisionType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

**DateTimePrecision**要素は、SOAP ヘッダーにあります。 
  
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 指定可能な値は次のいずれかです。
  
- 秒
    
- (
    
## <a name="remarks"></a>注釈

**DateTimePrecision**要素を "Seconds" に設定した SOAP ヘッダーを使用すると、日付/時刻の値が最も近い秒 (00:00:00) に戻されます。 "Milliseconds" が使用されている場合は、日付/時刻値が最も近いミリ秒 (00:00: 00.0000) に返されます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

