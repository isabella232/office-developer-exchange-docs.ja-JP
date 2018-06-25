---
title: ReplyBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyBody
api_type:
- schema
ms.assetid: bb184144-3e4b-4419-a883-cc9fab1085e6
description: ReplyBody 要素には、Office (OOF) メッセージと、メッセージに使用する言語が含まれています。
ms.openlocfilehash: 8400dda1ee810781e129fcc44fd3cd5d6c15cbbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833116"
---
# <a name="replybody"></a>ReplyBody

**ReplyBody**要素には、Office (OOF) メッセージと、メッセージに使用する言語が含まれています。 
  
```XML
<ReplyBody xml:lang="">
   <Message/>
</ReplyBody>
```

 **ReplyBody**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|xml:lang  <br/> |**ReplyBody**内容で使用する言語を指定します。 この属性は、省略可能です。 この属性に指定できる値は、IETF RFC 3066 で定義されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[メッセージ (可用性)](message-availability.md) <br/> |不在 (oof) の応答が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[OutOfOffice](outofoffice.md) <br/> |不在時の応答メッセージとメールボックスの応答メッセージを送信するための継続時間を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素は必須です。
  
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

