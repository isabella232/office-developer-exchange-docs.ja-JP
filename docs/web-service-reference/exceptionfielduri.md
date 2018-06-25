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
description: ExceptionFieldURI 要素は、要求内の特定のエラーを識別します。 この要素を MessageXml ノードにエラー応答の一部としてのみ使用します。
ms.openlocfilehash: 79909405179cec0d0b86ad12bf52031e1daeb790
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760350"
---
# <a name="exceptionfielduri"></a>ExceptionFieldURI

**ExceptionFieldURI**要素は、要求内の特定のエラーを識別します。 この要素を[MessageXml](messagexml.md)ノードにエラー応答の一部としてのみ使用します。 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 **ExceptionPropertyURIType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**FieldURI** <br/> |定期的なアイテムのプロパティを識別します。 この属性は、必要があります。  <br/> |
   
#### <a name="fielduri-attribute"></a>FieldURI 属性

|**値**|**説明**|
|:-----|:-----|
|添付ファイルの名前。  <br/> |エラーが含まれていると添付ファイル名を識別します。  <br/> |
|: コンテンツ タイプの添付ファイル  <br/> |エラーが含まれているコンテンツの種類を識別します。  <br/> |
|添付ファイルのコンテンツ。  <br/> |エラーがあること、コンテンツを識別します。  <br/> |
|定期的な月。  <br/> |月] フィールドにエラーがあることを識別します。  <br/> |
|定期的なアイテム: DayOfWeekIndex  <br/> |日曜日のインデックス エラーがあることを識別します。  <br/> |
|DaysOfWeek の定期的なアイテム。  <br/> |DaysOfWeek プロパティ エラーがあることを識別します。  <br/> |
|DayOfMonth の定期的なアイテム。  <br/> |DayOfMonth エラーがあることを識別します。  <br/> |
|繰り返しの間隔:  <br/> |エラーが含まれているとの間隔を指定します。  <br/> |
|定期的なアイテム: NumberOfOccurrences  <br/> |エラーがあることの出現回数を指定します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

