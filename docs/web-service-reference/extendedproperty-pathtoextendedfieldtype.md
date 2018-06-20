---
title: ExtendedProperty (PathToExtendedFieldType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa620b48-2ce3-437d-b51e-541247eea1d9
description: ExtendedProperty 要素は、統合連絡先ストアの拡張プロパティを指定します。
ms.openlocfilehash: 7541fa6330ee96f7791febfabc672dbcf0e95b54
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760419"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a>ExtendedProperty (PathToExtendedFieldType)

**ExtendedProperty**要素は、統合連絡先ストアの拡張プロパティを指定します。 
  
```xml
<ExtendedProperty DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" FieldURI="">
</ExtendedProperty>
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|DistinguishedPropertySetId  <br/> |識別プロパティ セットの識別子を示します。 この属性は、省略可能です。  <br/> |
|PropertySetId  <br/> |GUID プロパティ セットの識別子を示します。 この属性は、省略可能です。  <br/> |
|PropertyTag  <br/> | 型部分を差し引いたプロパティ タグを表します。<br/><br/>表現の 2 つのオプションがあります。  <br/><br/>-16 進数: 0x3fa4  <br/>0 ~ 65535 の 10 進数。<br/><br/>  この属性は、省略可能です。  <br/> |
|PropertyName  <br/> |プロパティ名を示す文字列です。 この属性は、省略可能です。  <br/> |
|PropertyId  <br/> |プロパティの識別子を示す整数。 この属性は、省略可能です。  <br/> |
|PropertyType  <br/> |プロパティの型を示します。 この属性は、必要があります。  <br/> |
|FieldURI  <br/> |統一リソース識別子 (URI) のフィールドを示します。 この属性は、必要があります。 使用可能な値は、 [FieldURI](fielduri.md)要素を参照してください。  <br/> |
   
#### <a name="distinguishedpropertysetid"></a>DistinguishedPropertySetId

|**値**|**説明**|
|:-----|:-----|
|会議  <br/> |会議を示しています。  <br/> |
|Appointment  <br/> |予定を示します。  <br/> |
|Common  <br/> |共通のプロパティ セットを示します。  <br/> |
|PublicStrings  <br/> |パブリック文字列を示します。  <br/> |
|Address  <br/> |アドレスを示します。  <br/> |
|InternetHeaders  <br/> |インターネット ヘッダーを示します。  <br/> |
|CalendarAssistant  <br/> |予定表のアシスタントを示します。  <br/> |
|UnifiedMessaging  <br/> |ユニファイド メッセージングを示します。  <br/> |
|タスク  <br/> |タスクを示します。  <br/> |
   
#### <a name="propertytype"></a>PropertyType

|**値**|**説明**|
|:-----|:-----|
|ApplicationTime  <br/> |アプリケーション時刻を示します。  <br/> |
|ApplicationTimeArray  <br/> |アプリケーション時間の配列を示します。  <br/> |
|バイナリ型 (Binary)  <br/> |バイナリ値を示します。  <br/> |
|BinaryArray  <br/> |バイナリ値の配列を示します。  <br/> |
|ブール型  <br/> |ブール値を示します。  <br/> |
|CLSID  <br/> |CLSID を指定します。  <br/> |
|CLSIDArray  <br/> |Clsid の配列を示します。  <br/> |
|通貨型 (Currency)  <br/> |通貨値を示します。  <br/> |
|CurrencyArray  <br/> |通貨の値の配列を示します。  <br/> |
|倍精度浮動小数点型 (Double)  <br/> |**二重**のことを示します。  <br/> |
|DoubleArray  <br/> |**Double**値の配列を示します。  <br/> |
|エラー  <br/> |エラーを示します。 これは、エラー報告用です。 制限や値の設定を取得または使用できません。  <br/> |
|浮動小数点型 (Float)  <br/> |**浮動小数点数**を示します。  <br/> |
|FloatArray  <br/> |**Float**値の配列を示します。  <br/> |
|整数型 (Integer)  <br/> |整数を示します。  <br/> |
|IntegerArray  <br/> |整数の配列を示します。  <br/> |
|Long 型 (Long)  <br/> |**長い**ことを示します。  <br/> |
|LongArray  <br/> |**Long**値の配列を示します。  <br/> |
|Null  <br/> |Null 値を示します。 これは、エラー報告用です。 制限や値の設定を取得または使用できません。  <br/> |
|オブジェクト  <br/> |オブジェクトを示します。 これは、エラー報告用です。 制限や値の設定を取得または使用できません。  <br/> |
|ObjectArray  <br/> |オブジェクトの配列を示します。 これは、エラー報告用です。 制限や値の設定を取得または使用できません。  <br/> |
|長い形式の日付 (スラッシュ区切り)  <br/> |**短い**ことを示します。  <br/> |
|ShortArray  <br/> |**Short**値の配列を示します。  <br/> |
|SystemTime  <br/> |システム時刻の値を示します。  <br/> |
|SystemTimeArray  <br/> |システム時刻の値の配列を示します。  <br/> |
|String  <br/> |文字列を示します。  <br/> |
|自己責任で使用  <br/> |文字列の配列を示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |拡張 MAPI プロパティを識別します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

