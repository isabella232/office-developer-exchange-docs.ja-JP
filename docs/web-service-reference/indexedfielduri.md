---
title: IndexedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedFieldURI
api_type:
- schema
ms.assetid: 5c9cd0b5-7eca-480a-8730-fe98b1779afa
description: IndexedFieldURI 要素は、辞書の個々のメンバーを識別します。
ms.openlocfilehash: f794d9970590417d916925f7258b28d4f0920d0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467019"
---
# <a name="indexedfielduri"></a>IndexedFieldURI

**IndexedFieldURI**要素は、辞書の個々のメンバーを識別します。 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 **PathToIndexedFieldType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**FieldURI** <br/> |返すメンバーを含むディクショナリを識別します。 この属性は必須です。  <br/> |
|**FieldIndex** <br/> |取得する辞書のメンバを識別します。 この属性は必須です。  <br/> |
   
#### <a name="fielduri-attribute"></a>FieldURI 属性

|**値**|**説明**|
|:-----|:-----|
|アイテム: InternetMessageHeader  <br/> |アイテムのメッセージヘッダーを表します。  <br/> |
|連絡先: ImAddress  <br/> |連絡先のインスタントメッセージングアドレスを表します。  <br/> |
|連絡先: PhysicalAddress: ストリート  <br/> |連絡先の住所を表します。  <br/> |
|連絡先: PhysicalAddress: City  <br/> |連絡先の市町村を表します。  <br/> |
|連絡先: PhysicalAddress: State  <br/> |連絡先の状態を表します。  <br/> |
|連絡先: PhysicalAddress: Country  <br/> |連絡先の国/地域を表します。  <br/> |
|連絡先: PhysicalAddress: 郵便番号  <br/> |連絡先の郵便番号を表します。  <br/> |
|連絡先: PhoneNumber  <br/> |連絡先の電話番号を表します。  <br/> |
|連絡先: EmailAddress  <br/> |連絡先の電子メールアドレスを表します。  <br/> |
|distributionlist: Members: Member  <br/> |配布リストのメンバーを表します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdditionalProperties](additionalproperties.md) <br/> |取得、設定、または作成する追加のプロパティを識別します。  <br/> |
|[AggregateOn](aggregateon.md) <br/> |グループ化された FindItem 結果セットのグループ化されたアイテムの順序を決定するために使用されるプロパティを表します。  <br/> |
|[GroupBy](groupby.md) <br/> |FindItem クエリの任意のグループを指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

