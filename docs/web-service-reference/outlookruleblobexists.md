---
title: OutlookRuleBlobExists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutlookRuleBlobExists
api_type:
- schema
ms.assetid: ae1bc448-deb9-4b5b-ab38-4b276abcb650
description: OutlookRuleBlobExists 要素は、Microsoft Outlook のルール blob がユーザーのメールボックス内に存在するかどうかを示します。
ms.openlocfilehash: 6a5c2a2ec0246d38b22279b86772972ea81922c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529029"
---
# <a name="outlookruleblobexists"></a>OutlookRuleBlobExists

**Outlookruleblobexists**要素は、Microsoft Outlook のルール blob がユーザーのメールボックス内に存在するかどうかを示します。 
  
[Get受信規則の応答](getinboxrulesresponse.md)
  
[OutlookRuleBlobExists](outlookruleblobexists.md)
  
```XML
<OutlookRuleBlobExists>true | false</OutlookRuleBlobExists>
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
|[Get受信規則の応答](getinboxrulesresponse.md) <br/> |[Get受信トレイの操作](getinboxrules-operation.md)要求への応答を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値が**true の場合**は、Outlook ルール blob が存在することを示します。 テキスト値が**false**の場合は、Outlook ルール blob が存在しないことを示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

