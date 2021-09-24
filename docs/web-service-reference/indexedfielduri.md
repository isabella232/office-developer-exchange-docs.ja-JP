---
title: IndexedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IndexedFieldURI
api_type:
- schema
ms.assetid: 5c9cd0b5-7eca-480a-8730-fe98b1779afa
description: IndexedFieldURI 要素は、辞書の個々のメンバーを識別します。
ms.openlocfilehash: 851d0d4296e926ab21e5bd1b842d5a215c27308a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539627"
---
# <a name="indexedfielduri"></a>IndexedFieldURI

**IndexedFieldURI 要素** は、辞書の個々のメンバーを識別します。 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 **PathToIndexedFieldType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**FieldURI** <br/> |返すメンバーを含む辞書を識別します。 この属性は必須です。  <br/> |
|**FieldIndex** <br/> |返す辞書のメンバーを識別します。 この属性は必須です。  <br/> |
   
#### <a name="fielduri-attribute"></a>FieldURI 属性

|**値**|**説明**|
|:-----|:-----|
|item:InternetMessageHeader  <br/> |アイテムのメッセージ ヘッダーを表します。  <br/> |
|contacts:ImAddress  <br/> |連絡先のインスタント メッセージング アドレスを表します。  <br/> |
|contacts:PhysicalAddress:Street  <br/> |連絡先の住所を表します。  <br/> |
|contacts:PhysicalAddress:City  <br/> |連絡先の都市を表します。  <br/> |
|contacts:PhysicalAddress:State  <br/> |連絡先の状態を表します。  <br/> |
|contacts:PhysicalAddress:Country  <br/> |連絡先の国/地域を表します。  <br/> |
|contacts:PhysicalAddress:PostalCode  <br/> |連絡先の郵便番号を表します。  <br/> |
|contacts:PhoneNumber  <br/> |連絡先の電話番号を表します。  <br/> |
|contacts:EmailAddress  <br/> |連絡先の電子メール アドレスを表します。  <br/> |
|distributionlist:Members:Member  <br/> |配布リストのメンバーを表します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdditionalProperties](additionalproperties.md) <br/> |取得、設定、または作成する追加のプロパティを識別します。  <br/> |
|[AggregateOn](aggregateon.md) <br/> |グループ化された FindItem 結果セットのグループ化されたアイテムの順序を決定するために使用されるプロパティを表します。  <br/> |
|[GroupBy](groupby.md) <br/> |FindItem クエリの任意のグループ化を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

