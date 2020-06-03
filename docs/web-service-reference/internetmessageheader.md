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
description: InternetMessageHeader 要素は、ヘッダーコレクション内の指定されたヘッダーのインターネットメッセージヘッダーを表します。 インターネットメッセージヘッダーのコレクション全体を取得するには、PR_TRANSPORT_MESSAGE_HEADERS プロパティを使用します。 EWS およびインターネットメッセージヘッダーの詳細については、「EWS、MIME、および不足しているインターネットメッセージヘッダーのインターネットメッセージヘッダーを取得する」を参照してください。
ms.openlocfilehash: 7b662617e0b1a1fcdcce3449b729485ba6e0956b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459308"
---
# <a name="internetmessageheader"></a>InternetMessageHeader

**Internetmessageheader**要素は、ヘッダーコレクション内の指定されたヘッダーのインターネットメッセージヘッダーを表します。 インターネットメッセージヘッダーのコレクション全体を取得するには、 **PR_TRANSPORT_MESSAGE_HEADERS**プロパティを使用します。 EWS およびインターネットメッセージヘッダーの詳細については、「 [ews、MIME、および不足しているインターネットメッセージ](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)ヘッダーのインターネットメッセージヘッダーを取得する」を参照してください。
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 **InternetHeaderType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ヘッド Ername** <br/> |ヘッダー名を識別します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |メールボックス内のアイテムに含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、ヘッダーの値を表します。
  
## <a name="remarks"></a>注釈

**PR_TRANSPORT_MESSAGE_HEADERS**プロパティの EWS マネージ API 拡張プロパティの定義を次に示します。 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

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


[EWS、MIME、および欠落しているインターネット メッセージ ヘッダー](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

