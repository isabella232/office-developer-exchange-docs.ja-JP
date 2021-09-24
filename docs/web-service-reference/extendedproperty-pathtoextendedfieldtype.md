---
title: ExtendedProperty (PathToExtendedFieldType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fa620b48-2ce3-437d-b51e-541247eea1d9
description: ExtendedProperty 要素は、統合連絡先ストアの拡張プロパティを指定します。
ms.openlocfilehash: 5cb320e15d3a01c542907048357d1ef0cc78f96a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530760"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a>ExtendedProperty (PathToExtendedFieldType)

**ExtendedProperty 要素** は、統合連絡先ストアの拡張プロパティを指定します。 
  
```xml
<ExtendedProperty DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" FieldURI="">
</ExtendedProperty>
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|DistinguishedPropertySetId  <br/> |識別プロパティ セット識別子を示します。 この属性は省略可能です。  <br/> |
|PropertySetId  <br/> |GUID プロパティ セット識別子を示します。 この属性は省略可能です。  <br/> |
|PropertyTag  <br/> | プロパティ タグから型パーツを引いた値を表します。<br/><br/>表現には、次の 2 つのオプションがあります。  <br/><br/>- 16 進数: 0x3fa4  <br/>- Decimal: 0 ~ 65535<br/><br/>  この属性は省略可能です。  <br/> |
|PropertyName  <br/> |プロパティ名を示す文字列。 この属性は省略可能です。  <br/> |
|PropertyId  <br/> |プロパティ識別子を示す整数。 この属性は省略可能です。  <br/> |
|PropertyType  <br/> |プロパティの種類を示します。 この属性は必須です。  <br/> |
|FieldURI  <br/> |[統一リソース識別子] (URI) フィールドを示します。 この属性は必須です。 可能な値については [、FieldURI 要素を参照](fielduri.md) してください。  <br/> |
   
#### <a name="distinguishedpropertysetid"></a>DistinguishedPropertySetId

|**値**|**説明**|
|:-----|:-----|
|会議  <br/> |会議を示します。  <br/> |
|Appointment  <br/> |予定を示します。  <br/> |
|共通  <br/> |共通のプロパティ セットを示します。  <br/> |
|PublicStrings  <br/> |パブリック文字列を示します。  <br/> |
|Address  <br/> |アドレスを示します。  <br/> |
|InternetHeaders  <br/> |インターネット ヘッダーを示します。  <br/> |
|CalendarAssistant  <br/> |予定表アシスタントを示します。  <br/> |
|UnifiedMessaging  <br/> |ユニファイド メッセージングを示します。  <br/> |
|タスク  <br/> |タスクを示します。  <br/> |
   
#### <a name="propertytype"></a>PropertyType

|**値**|**説明**|
|:-----|:-----|
|ApplicationTime  <br/> |アプリケーションの時刻を示します。  <br/> |
|ApplicationTimeArray  <br/> |アプリケーションの時間の配列を示します。  <br/> |
|Binary  <br/> |バイナリ値を示します。  <br/> |
|BinaryArray  <br/> |バイナリ値の配列を示します。  <br/> |
|ブール型  <br/> |ブール値を示します。  <br/> |
|CLSID  <br/> |CLSID を示します。  <br/> |
|CLSIDArray  <br/> |CLSID の配列を示します。  <br/> |
|通貨  <br/> |通貨の値を示します。  <br/> |
|CurrencyArray  <br/> |通貨値の配列を示します。  <br/> |
|Double  <br/> |倍数を示 **します**。  <br/> |
|DoubleArray  <br/> |倍数の値の配列 **を示** します。  <br/> |
|Error  <br/> |エラーを示します。 これは、エラー報告を目的とします。 制限や値の取得または設定には使用できません。  <br/> |
|浮動小数点数  <br/> |浮動小数点数を示 **します**。  <br/> |
|FloatArray  <br/> |浮動小数点値の配列 **を示** します。  <br/> |
|整数  <br/> |整数を示します。  <br/> |
|IntegerArray  <br/> |整数の配列を示します。  <br/> |
|Long  <br/> |長いを示 **します**。  <br/> |
|LongArray  <br/> |長い値の配列 **を示** します。  <br/> |
|Null  <br/> |null 値を示します。 これは、エラー報告を目的とします。 制限や値の取得または設定には使用できません。  <br/> |
|オブジェクト  <br/> |オブジェクトを示します。 これは、エラー報告を目的とします。 制限や値の取得または設定には使用できません。  <br/> |
|ObjectArray  <br/> |オブジェクトの配列を示します。 これは、エラー報告を目的とします。 制限や値の取得または設定には使用できません。  <br/> |
|長い形式の日付 (スラッシュ区切り)  <br/> |短い値を **示します**。  <br/> |
|ShortArray  <br/> |短い値の配列 **を示** します。  <br/> |
|SystemTime  <br/> |システム時刻の値を示します。  <br/> |
|SystemTimeArray  <br/> |システム時刻の値の配列を示します。  <br/> |
|String  <br/> |文字列を示します。  <br/> |
|StringArray  <br/> |文字列の配列を示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |拡張 MAPI プロパティを識別します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

