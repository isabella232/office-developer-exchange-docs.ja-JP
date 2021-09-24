---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: DateTimePrecision 要素は、返される日付/時刻の値の精度を指定します。
ms.openlocfilehash: 075e37bfdd2c61f56352e000ef6cc5810dd81bbb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535711"
---
# <a name="datetimeprecision"></a>DateTimePrecision

**DateTimePrecision 要素は**、返される日付/時刻の値の精度を指定します。 
  
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

**DateTimePrecision 要素** は SOAP ヘッダー内に存在します。 
  
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 指定可能な値は次のいずれかです。
  
- 秒
    
- ミリ秒
    
## <a name="remarks"></a>注釈

**DateTimePrecision 要素が "Seconds"** に設定された SOAP ヘッダーを使用すると、日付/時刻の値は最も近い秒 (00:00:00) に返されます。 "ミリ秒" を使用すると、日付/時刻の値が最も近いミリ秒 (00:00:00.0000) に返されます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

