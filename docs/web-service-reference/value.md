---
title: 値
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Value
api_type:
- schema
ms.assetid: 9a30cadd-909e-41b1-b4e9-291643dd89c6
description: Value 要素には、拡張プロパティの値が含まれる。
ms.openlocfilehash: dc9d81a17896e730a5140a097574faa7619576d1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513949"
---
# <a name="value"></a>値

**Value 要素** には、拡張プロパティの値が含まれる。 
  
```xml
<Value/>
```

**String**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[値](values.md) <br/> |拡張プロパティの値のコレクションを格納します。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーとアイテムの拡張プロパティを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ExtendedFieldURI の PropertyType 属性で示される型と互換性がある必要があります。
  
## <a name="remarks"></a>注釈

Value **要素は** 、単一の拡張プロパティ インスタンスと複数値の拡張プロパティ インスタンスの両方で発生する可能性があります。 単一値のインスタンスの場合 [、ExtendedProperty](extendedproperty.md) 要素の直接の子として存在します。 複数値を持つインスタンスの場合、Values コレクションの直接の子として **存在** します。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

