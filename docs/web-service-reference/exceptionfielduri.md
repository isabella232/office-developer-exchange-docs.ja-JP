---
title: ExceptionFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExceptionFieldURI
api_type:
- schema
ms.assetid: 7afda93a-0f8c-4c9e-8e09-f1b0bfc928bf
description: ExceptionFieldURI 要素は、要求内の特定のエラーを識別します。 この要素は、MessageXml ノードのエラー応答の一部としてのみ使用されます。
ms.openlocfilehash: 7368fd51e8eca2081b1fd50c86bce9ffa469c6b1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524330"
---
# <a name="exceptionfielduri"></a>ExceptionFieldURI

**ExceptionFieldURI 要素** は、要求内の特定のエラーを識別します。 この要素は、MessageXml ノードのエラー応答の一部 [としてのみ使用](messagexml.md) されます。 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 **ExceptionPropertyURIType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**FieldURI** <br/> |定期的なアイテムの出現のプロパティを識別します。 この属性は必須です。  <br/> |
   
#### <a name="fielduri-attribute"></a>FieldURI 属性

|**値**|**説明**|
|:-----|:-----|
|attachment:Name  <br/> |添付ファイル名にエラーが含まれていると識別します。  <br/> |
|attachment:ContentType  <br/> |エラーを含むコンテンツ タイプを識別します。  <br/> |
|attachment:Content  <br/> |エラーを含むコンテンツを識別します。  <br/> |
|recurrence:Month  <br/> |月フィールドにエラーが含まれていると識別します。  <br/> |
|recurrence:DayOfWeekIndex  <br/> |日のインデックスをエラーを含むとして識別します。  <br/> |
|recurrence:DaysOfWeek  <br/> |エラーを含む DaysOfWeek プロパティを識別します。  <br/> |
|recurrence:DayOfMonth  <br/> |エラーを含む DayOfMonth を識別します。  <br/> |
|recurrence:Interval  <br/> |間隔をエラーを含むとして識別します。  <br/> |
|recurrence:NumberOfOccurrences  <br/> |発生回数をエラーを含むとして識別します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

