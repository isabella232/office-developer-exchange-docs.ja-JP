---
title: ItemHoldPeriod
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30369db5-4d45-40e8-bc83-3236667fc404
description: ItemHoldPeriod 要素は、メールボックスクエリに一致するコンテンツを保持する時間の長さを指定します。
ms.openlocfilehash: 185666b72cc96dd88605b7baa6433d070e7ebc91
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452287"
---
# <a name="itemholdperiod"></a>ItemHoldPeriod

**ItemHoldPeriod**要素は、メールボックスクエリに一致するコンテンツを保持する時間の長さを指定します。 
  
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

テキスト値には、"無制限" または任意の[Timespan](https://msdn.microsoft.com/library/1ecy8h51%28v=vs.110%29.aspx)値の文字列値を指定できます。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[SetHoldOnMailboxes](setholdonmailboxes.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

