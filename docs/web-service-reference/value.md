---
title: 値
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: 9a30cadd-909e-41b1-b4e9-291643dd89c6
description: 値の要素には、拡張プロパティの値が含まれています。
ms.openlocfilehash: 4b8674d267b78f0384f9457e794e88ace8234826
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839984"
---
# <a name="value"></a>値

**値**の要素には、拡張プロパティの値が含まれています。 
  
```xml
<Value/>
```

**文字列型 (String)**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Values](values.md) <br/> |拡張プロパティの値のコレクションが含まれています。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーおよびアイテムの拡張プロパティを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ExtendedFieldURI の登録するときの属性によって指定されている型との互換性である必要があります。
  
## <a name="remarks"></a>備考

**値**要素は、両方の拡張プロパティの 1 つと複数値を持つインスタンスで発生します。 単一の値のインスタンスでは、 [ExtendedProperty](extendedproperty.md)要素の直接の子として存在します。 複数値を持つインスタンスの**値**のコレクションの直接の子として存在します。 
  
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

