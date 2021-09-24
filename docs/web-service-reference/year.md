---
title: Year
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Year
api_type:
- schema
ms.assetid: 93bf2847-53fa-496c-9a1e-dc9a9ffd0b9f
description: Year 要素は、年に応じて変化するタイム ゾーンを定義するために使用されます。 この要素は省略できます。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: 80b4ce642a7a08631140e583fb9d92143f485ea3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509281"
---
# <a name="year"></a>Year

Year **要素** は、年に応じて変化するタイム ゾーンを定義するために使用されます。 この要素は省略できます。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
```xml
<Year/>
```

**string**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> |Bias (UTC) 要素で表される協定世界時 [(UTC)](bias-utc.md) を基準にした時刻からのオフセットを表します。  <br/> |
|[DaylightTime](daylighttime.md) <br/> |夏時間が観測される地域の Bias (UTC) 要素で表される協定世界時 [(UTC)](bias-utc.md) を基準にした時刻からのオフセットを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Year 要素は、年を表す文字列を受け取ります。 年形式は YYYY です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

