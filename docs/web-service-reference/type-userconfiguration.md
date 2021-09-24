---
title: Type (UserConfiguration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Type
api_type:
- schema
ms.assetid: d09a9621-6950-451a-90dc-920af9cab35c
description: Type 要素は、ディクショナリ オブジェクトの種類を指定します。
ms.openlocfilehash: f0bafa9023a42fdf8464891e8df7931a0766b416
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538731"
---
# <a name="type-userconfiguration"></a>Type (UserConfiguration)

**Type 要素は**、ディクショナリ オブジェクトの種類を指定します。 
  
```xml
<Type>DateTime or Boolean or Byte or String or Integer32 or UnsignedInteger32 or Integer64 or UnsignedInteger64 or StringArray or ByteArray</Type> 
```

 **UserConfigurationDictionaryObjectTypesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DictionaryKey](dictionarykey.md) <br/> |ディクショナリ プロパティの辞書キーを指定します。  <br/> |
|[DictionaryValue](dictionaryvalue.md) <br/> |ディクショナリ プロパティの辞書値を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、Type** 要素に使用できる値を示します。 
  
**Type 要素の値**

|**値**|**説明**|
|:-----|:-----|
|DateTime  <br/> ||
|ブール型  <br/> ||
|バイト型 (Byte)  <br/> ||
|String  <br/> ||
|Integer32  <br/> ||
|UnsignedInteger32  <br/> ||
|Integer64  <br/> ||
|UnsignedInteger64  <br/> ||
|StringArray  <br/> ||
|ByteArray  <br/> ||
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

