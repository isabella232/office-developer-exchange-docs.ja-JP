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
ms.openlocfilehash: f6c283d5cce3bc927662ad0d9c796c0589e7054c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460142"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a>ExtendedProperty (PathToExtendedFieldType)

**Extendedproperty**要素は、統合連絡先ストアの拡張プロパティを指定します。 
  
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
|DistinguishedPropertySetId  <br/> |識別プロパティセット識別子を示します。 この属性は省略可能です。  <br/> |
|PropertySetId  <br/> |GUID プロパティセット識別子を示します。 この属性は省略可能です。  <br/> |
|PropertyTag  <br/> | プロパティタグから type part を引いたものを表します。<br/><br/>表現には、次の2つのオプションがあります。  <br/><br/>-16 進: 0x3fa4  <br/>-10 進: 0-65535<br/><br/>  この属性は省略可能です。  <br/> |
|PropertyName  <br/> |プロパティ名を示す文字列。 この属性は省略可能です。  <br/> |
|PropertyId  <br/> |プロパティ識別子を示す整数。 この属性は省略可能です。  <br/> |
|Recordtype  <br/> |プロパティの種類を示します。 この属性は必須です。  <br/> |
|FieldURI  <br/> |フィールド URI (Uniform Resource Identifier) を示します。 この属性は必須です。 可能な値については、 [FieldURI](fielduri.md)要素を参照してください。  <br/> |
   
#### <a name="distinguishedpropertysetid"></a>DistinguishedPropertySetId

|**値**|**説明**|
|:-----|:-----|
|会議  <br/> |会議を示します。  <br/> |
|Appointment  <br/> |予定を示します。  <br/> |
|共通  <br/> |Common プロパティセットを示します。  <br/> |
|PublicStrings  <br/> |パブリック文字列を示します。  <br/> |
|Address  <br/> |アドレスを示します。  <br/> |
|InternetHeaders  <br/> |インターネットヘッダーを示します。  <br/> |
|CalendarAssistant  <br/> |カレンダーアシスタントを示します。  <br/> |
|UnifiedMessaging  <br/> |ユニファイドメッセージングを示します。  <br/> |
|タスク  <br/> |タスクを示します。  <br/> |
   
#### <a name="propertytype"></a>Recordtype

|**値**|**説明**|
|:-----|:-----|
|ApplicationTime  <br/> |アプリケーション時間を示します。  <br/> |
|ApplicationTimeArray  <br/> |アプリケーション時間の配列を示します。  <br/> |
|バイナリ  <br/> |バイナリ値を示します。  <br/> |
|BinaryArray  <br/> |バイナリ値の配列を示します。  <br/> |
|ブール型  <br/> |ブール値を示します。  <br/> |
|CLSID  <br/> |CLSID を示します。  <br/> |
|CLSIDArray  <br/> |Clsid の配列を示します。  <br/> |
|通貨  <br/> |通貨値を示します。  <br/> |
|CurrencyArray  <br/> |通貨値の配列を示します。  <br/> |
|倍精度浮動小数点数  <br/> |**倍精度浮動小数点**型を示します。  <br/> |
|DoubleArray  <br/> |**倍精度浮動小数点**型の値の配列を示します。  <br/> |
|Error  <br/> |エラーを示します。 これはエラーレポートのためのものです。 制限で、または値を取得または設定するために使用することはできません。  <br/> |
|浮動小数点数  <br/> |**Float**を示します。  <br/> |
|FloatArray  <br/> |**Float**値の配列を示します。  <br/> |
|整数  <br/> |整数を示します。  <br/> |
|整数配列  <br/> |整数の配列を示します。  <br/> |
|Long  <br/> |**Long**を示します。  <br/> |
|LongArray  <br/> |**長整数型 (long)** の値の配列を示します。  <br/> |
|Null  <br/> |Null 値を示します。 これはエラーレポートのためのものです。 制限で、または値を取得または設定するために使用することはできません。  <br/> |
|オブジェクト  <br/> |オブジェクトを示します。 これはエラーレポートのためのものです。 制限で、または値を取得または設定するために使用することはできません。  <br/> |
|ObjectArray  <br/> |オブジェクトの配列を示します。 これはエラーレポートのためのものです。 制限で、または値を取得または設定するために使用することはできません。  <br/> |
|長い形式の日付 (スラッシュ区切り)  <br/> |**Short**を示します。  <br/> |
|Short 配列  <br/> |**Short**値の配列を示します。  <br/> |
|SystemTime  <br/> |システム時間の値を示します。  <br/> |
|SystemTimeArray  <br/> |システム時間の値の配列を示します。  <br/> |
|文字列  <br/> |文字列を示します。  <br/> |
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
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

