---
title: NotSentToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- NotSentToMe
api_type:
- schema
ms.assetid: 7cb63269-622c-4198-9a21-f5a021bf6901
description: NotSentToMe 要素は、メールボックスの所有者が、条件または例外を適用するために、受信メッセージの ToRecipients プロパティに含めなければならないかどうかを示します。
ms.openlocfilehash: f3c2994778298c1c8a27626fb0d4b32d6d2963cb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518107"
---
# <a name="notsenttome"></a>NotSentToMe

**NotSentToMe** 要素は、メールボックスの所有者が、条件または例外を適用するために、受信メッセージの **ToRecipients** プロパティに含めなければならないかどうかを示します。 
  
```xml
<NotSentToMe>true | false</NotSentToMe>
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
|[例外](exceptions.md) <br/> |受信トレイ ルールで使用可能なすべてのルール例外条件を表す例外を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

true **のテキスト値** は、メールボックスの所有者が、条件または例外を適用するために、受信メッセージの **ToRecipients** プロパティに含めずにいなければならないと示します。 false の **値は** 、メールボックスの所有者が、条件または例外を適用するために、受信メッセージの **ToRecipients** プロパティに含む必要があります。 
  
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

