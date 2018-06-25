---
title: InternetMessageHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeader
api_type:
- schema
ms.assetid: c70675f8-6feb-4c89-ba48-bce0479b308b
description: InternetMessageHeader 要素は、ヘッダー コレクション内の指定したヘッダーのインターネット メッセージ ヘッダーを表します。 インターネット メッセージ ヘッダーのコレクション全体を取得するには、PR_TRANSPORT_MESSAGE_HEADERS プロパティを使用します。 EWS およびインターネット メッセージ ヘッダーの詳細については、EWS、MIME、および不足しているインターネットの seeGetting のインターネット メッセージ ヘッダー メッセージ ヘッダーを使用します。
ms.openlocfilehash: 9457cdabe99c0adcb8183cbc039cc86db881fec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831952"
---
# <a name="internetmessageheader"></a>InternetMessageHeader

**InternetMessageHeader**要素は、ヘッダー コレクション内の指定したヘッダーのインターネット メッセージ ヘッダーを表します。 インターネット メッセージ ヘッダーのコレクション全体を取得するには、 **PR_TRANSPORT_MESSAGE_HEADERS**プロパティを使用します。 EWS およびインターネット メッセージ ヘッダーの詳細についてを参照してください["EWS、MIME、および不足しているインターネット メッセージ ヘッダー](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)の取得インターネット メッセージのヘッダーです。
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 **InternetHeaderType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**HeaderName** <br/> |ヘッダー名を識別します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |メールボックス内のアイテムに含まれるすべてのインターネット メッセージ ヘッダーのコレクションを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ヘッダーの値を表します。
  
## <a name="remarks"></a>備考

**PR_TRANSPORT_MESSAGE_HEADERS**プロパティのプロパティの定義を拡張する EWS マネージ API は、次のようにします。 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

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


[EWS、MIME、および不足しているインターネット メッセージのヘッダー](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)

