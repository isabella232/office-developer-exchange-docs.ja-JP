---
title: InternetMessageHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InternetMessageHeader
api_type:
- schema
ms.assetid: c70675f8-6feb-4c89-ba48-bce0479b308b
description: InternetMessageHeader 要素は、header コレクション内の特定のヘッダーのインターネット メッセージ ヘッダーを表します。 インターネット メッセージ ヘッダーのコレクション全体を取得するには、PR_TRANSPORT_MESSAGE_HEADERSプロパティを使用します。 EWS およびインターネット メッセージ ヘッダーの詳細については、「EWS、MIME、および不足しているインターネット メッセージ ヘッダーでインターネット メッセージ ヘッダーを取得する」を参照してください。
ms.openlocfilehash: 4b3072611e8a3debf87ce2a023f4f68ee4487185
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541085"
---
# <a name="internetmessageheader"></a>InternetMessageHeader

**InternetMessageHeader 要素** は、header コレクション内の特定のヘッダーのインターネット メッセージ ヘッダーを表します。 インターネット メッセージ ヘッダーのコレクション全体を取得するには、PR_TRANSPORT_MESSAGE_HEADERSプロパティ **を使用** します。 EWS およびインターネット メッセージ ヘッダーの詳細については [、「EWS、MIME、](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)および不足しているインターネット メッセージ ヘッダーでインターネット メッセージ ヘッダーを取得する」を参照してください。
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 **InternetHeaderType**
## <a name="attributes-and-elements"></a>属性と要素

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
  
## <a name="remarks"></a>注釈

次に、EWS マネージ API 拡張プロパティ定義を示します。PR_TRANSPORT_MESSAGE_HEADERS **します。** 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

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


[EWS、MIME、および欠落しているインターネット メッセージ ヘッダー](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

