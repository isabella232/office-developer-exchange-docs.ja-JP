---
title: '[開始日'
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cbb1320c-479e-4bd3-a462-4ab14c24b1c5
description: 開始要素は、メッセージが送信された日付を指定します。
ms.openlocfilehash: edc3f8ada87c64ccc3eeeb8a7467e7e050a30ce1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760613"
---
# <a name="fromdate"></a>[開始日

**開始**要素は、メッセージが送信された日付を指定します。 
  
```XML
<FromDate></FromDate>
```

 **dateTime**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindMailboxStatisticsByKeywords](findmailboxstatisticsbykeywords.md) <br/> |キーワードでメールボックスの統計情報を検索するための要求を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**開始**要素のテキスト値は、メッセージが送信されたときの日時です。 
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

