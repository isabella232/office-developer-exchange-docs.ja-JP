---
title: ItemHoldPeriod
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 30369db5-4d45-40e8-bc83-3236667fc404
description: ItemHoldPeriod 要素は、メールボックス クエリに一致するコンテンツを保持する時間を指定します。
ms.openlocfilehash: de56c410c876917bbe8d545c9ef4f38ee6948b21
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522853"
---
# <a name="itemholdperiod"></a>ItemHoldPeriod

**ItemHoldPeriod** 要素は、メールボックス クエリに一致するコンテンツを保持する時間を指定します。 
  
```XML
<ItemHoldPeriod/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>テキスト値

テキスト値には、"Unlimited" または任意の Timespan 値の [文字列値を指定](https://msdn.microsoft.com/library/1ecy8h51%28v=vs.110%29.aspx) できます。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[SetHoldOnMailboxes](setholdonmailboxes.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

