---
title: SubmitTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SubmitTime
api_type:
- schema
ms.assetid: 97e4b71e-f45c-4bdb-80f9-805934916c0f
description: SubmitTime 要素は、メッセージがサーバーに送信された時刻を表します。
ms.openlocfilehash: 8a6a70da6a59942b13f5000666fd7581ce65bf37
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537385"
---
# <a name="submittime"></a>SubmitTime

**SubmitTime** 要素は、メッセージがサーバーに送信された時刻を表します。 
  
```XML
<SubmitTime/>
```

 **dateTime**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageTrackingReport](messagetrackingreport.md) <br/> |[GetMessageTrackingReport](getmessagetrackingreport-operation.md)操作で返される 1 つのメッセージを格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、日付/時刻を表すテキスト値が必要です。
  
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



[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

