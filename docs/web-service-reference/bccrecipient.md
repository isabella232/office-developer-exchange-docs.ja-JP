---
title: BccRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- BccRecipient
api_type:
- schema
ms.assetid: 4ef0cff5-8a5a-4d76-9d2b-938774d8fc1b
description: BccRecipient 要素は、電子メール メッセージのブラインド カーボン コピー (Bcc) を受信する受信者を表します。
ms.openlocfilehash: 178606d9c27becbf6fea5e7a9a694fb67feadc49
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526866"
---
# <a name="bccrecipient"></a>BccRecipient

**BccRecipient** 要素は、電子メール メッセージのブラインド カーボン コピー (Bcc) を受信する受信者を表します。 
  
```XML
<BccRecipient>true | false</BccRecipient>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |受信者の 1 つのイベントの情報を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素には **、true** または false を **指定できます**。 true の値 **は** 、受信者がブラインド カーボン コピーされた状態を示します。false の **値は** 、受信者がブラインド カーボン コピーを行っていないかどうかを示します。 
  
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

