---
title: 型 (UserConfiguration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Type
api_type:
- schema
ms.assetid: d09a9621-6950-451a-90dc-920af9cab35c
description: 型の要素では、ディクショナリ オブジェクトの種類を指定します。
ms.openlocfilehash: 01729f0b5cb71989aef550abb08346cfe9a35789
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839761"
---
# <a name="type-userconfiguration"></a>型 (UserConfiguration)

**型**の要素では、ディクショナリ オブジェクトの種類を指定します。 
  
```xml
<Type>DateTime or Boolean or Byte or String or Integer32 or UnsignedInteger32 or Integer64 or UnsignedInteger64 or StringArray or ByteArray</Type> 
```

 **UserConfigurationDictionaryObjectTypesType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DictionaryKey](dictionarykey.md) <br/> |ディクショナリ プロパティのディクショナリのキーを指定します。  <br/> |
|[DictionaryValue](dictionaryvalue.md) <br/> |ディクショナリ プロパティのディクショナリの値を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**型**の要素の値を次の表に一覧します。 
  
**要素の種類の値**

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
|自己責任で使用  <br/> ||
|ByteArray  <br/> ||
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

