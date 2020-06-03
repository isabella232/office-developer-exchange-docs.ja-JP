---
title: ExceptionFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExceptionFieldURI
api_type:
- schema
ms.assetid: 7afda93a-0f8c-4c9e-8e09-f1b0bfc928bf
description: ExceptionFieldURI 要素は、要求の特定のエラーを識別します。 この要素は、MessageXml ノードでエラー応答の一部としてのみ使用されます。
ms.openlocfilehash: a47d44098f85d8bacb1e7a2c48a33e478e56c7ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454345"
---
# <a name="exceptionfielduri"></a>ExceptionFieldURI

**ExceptionFieldURI**要素は、要求の特定のエラーを識別します。 この要素は、 [MessageXml](messagexml.md)ノードでエラー応答の一部としてのみ使用されます。 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 **ExceptionPropertyURIType プロパティ**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**FieldURI** <br/> |定期的なアイテムの発生のプロパティを識別します。 この属性は必須です。  <br/> |
   
#### <a name="fielduri-attribute"></a>FieldURI 属性

|**値**|**説明**|
|:-----|:-----|
|添付ファイル: 名前  <br/> |エラーが含まれる添付ファイルの名前を識別します。  <br/> |
|添付ファイル: ContentType  <br/> |エラーが含まれるコンテンツタイプを識別します。  <br/> |
|添付ファイル: コンテンツ  <br/> |エラーを含むコンテンツを識別します。  <br/> |
|定期的な予定: 月  <br/> |エラーを含む month フィールドを識別します。  <br/> |
|定期的なアイテム: DayOfWeekIndex  <br/> |エラーが含まれる曜日インデックスを識別します。  <br/> |
|定期的なアイテム: DaysOfWeek  <br/> |エラーを含む DaysOfWeek プロパティを識別します。  <br/> |
|定期的なアイテム: DayOfMonth  <br/> |エラーを含む DayOfMonth を識別します。  <br/> |
|繰り返し: 間隔  <br/> |エラーを含む間隔を識別します。  <br/> |
|繰り返し: NumberOfOccurrences  <br/> |エラーを含むオカレンスの数を識別します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageXml](messagexml.md) <br/> |エラー応答に関する追加情報を提供します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

