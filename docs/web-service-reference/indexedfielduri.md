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
description: IndexedFieldURI 要素は、辞書の個々 のメンバーを識別します。
ms.openlocfilehash: 6a75e8855ecabf15ca31bb1e05d569c258a43b0b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831909"
---
# <a name="indexedfielduri"></a>IndexedFieldURI

**IndexedFieldURI**要素は、辞書の個々 のメンバーを識別します。 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 **PathToIndexedFieldType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**FieldURI** <br/> |返すメンバーを格納しているディクショナリを識別します。 この属性は、必要があります。  <br/> |
|**FieldIndex** <br/> |返すディクショナリのメンバーを識別します。 この属性は、必要があります。  <br/> |
   
#### <a name="fielduri-attribute"></a>FieldURI 属性

|**値**|**説明**|
|:-----|:-----|
|アイテム: InternetMessageHeader  <br/> |アイテムのメッセージのヘッダーを表します。  <br/> |
|連絡先: ImAddress  <br/> |インスタント メッセージの連絡先のアドレスを表します。  <br/> |
|連絡先: PhysicalAddress:Street  <br/> |連絡先の住所を表します。  <br/> |
|連絡先: PhysicalAddress:City  <br/> |連絡先の市区町村を表します。  <br/> |
|連絡先: PhysicalAddress:State  <br/> |連絡先の状態を表します。  <br/> |
|連絡先: PhysicalAddress:Country  <br/> |連絡先の国/地域を表します。  <br/> |
|連絡先: PhysicalAddress:PostalCode  <br/> |連絡先の郵便番号コードを表します。  <br/> |
|連絡先: 電話番号  <br/> |連絡先の電話番号を表します。  <br/> |
|EmailAddress の連絡先:  <br/> |連絡先の電子メール アドレスを表します。  <br/> |
|distributionlist:Members:Member  <br/> |配布リストのメンバーを表します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdditionalProperties](additionalproperties.md) <br/> |取得、設定、または作成する追加のプロパティを識別します。  <br/> |
|[AggregateOn](aggregateon.md) <br/> |グループ化された FindItem 結果セットをグループ化した項目の順序を決定するために使用されるプロパティを表します。  <br/> |
|[GroupBy](groupby.md) <br/> |FindItem クエリの任意のグループ化を指定します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

