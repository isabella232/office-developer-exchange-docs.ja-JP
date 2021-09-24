---
title: PhoneCallId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PhoneCallId
api_type:
- schema
ms.assetid: 79e31a4c-fc84-4802-8761-470df8d63694
description: PhoneCallId 要素は、電話の呼び出しの識別子を指定します。 この要素は必須です。
ms.openlocfilehash: 00b23c8b4023a6fef9c27295c8e023e5324b7026
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528320"
---
# <a name="phonecallid"></a>PhoneCallId

**PhoneCallId 要素** は、電話の呼び出しの識別子を指定します。 この要素は必須です。 
  
```xml
<PhoneCallId Id="" />
```

 **PhoneCallIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |切断する電話を識別します。 この属性は必須です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DisconnectPhoneCall](disconnectphonecall.md) <br/> |呼び出しを切断する要求を表します。  <br/> |
|[GetPhoneCallInformation](getphonecallinformation.md) <br/> |電話の通話情報を取得する要求を表します。  <br/> |
|[PlayOnPhoneResponse (Exchange Web サービス)](playonphoneresponse-exchange-web-services.md) <br/> |PlayOnPhone 要求に対する応答を定義します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

