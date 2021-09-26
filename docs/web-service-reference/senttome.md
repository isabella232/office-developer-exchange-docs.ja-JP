---
title: SentToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SentToMe
api_type:
- schema
ms.assetid: f18aecd1-ad33-41c3-b275-4ca648ce1da0
description: SentToMe 要素は、メールボックスの所有者が、条件または例外を適用するために受信メッセージの ToRecipients プロパティに含める必要があるかどうかを示します。
ms.openlocfilehash: 127dc69024d6344aaa22d131454a56ef074397e5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546064"
---
# <a name="senttome"></a>SentToMe

**SentToMe** 要素は、メールボックスの所有者が、条件または例外を適用するために受信メッセージの **ToRecipients** プロパティに含める必要があるかどうかを示します。 
  
```XML
<SentToMe>true | false</SentToMe>
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
|[条件](conditions.md) <br/> |満たされると、ルールのルール アクションをトリガーする条件を表します。  <br/> |
|[例外](exceptions.md) <br/> |受信トレイ ルールで使用可能なすべてのルール例外条件を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

true **のテキスト値** は、メールボックスの所有者が、条件または例外を適用するために受信メッセージの **ToRecipients** プロパティに含めなければならないかどうかを示します。 false の **値は** 、メールボックスの所有者が、条件または例外を適用するために、受信メッセージの **ToRecipients** プロパティに含めずにいなければならないと示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

