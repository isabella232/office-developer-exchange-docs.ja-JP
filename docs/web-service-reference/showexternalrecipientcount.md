---
title: Showexternal受信者カウント
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: Showexternalrecipients Count 要素は、GetMailTips ヒント操作のコンシューマーが、メッセージの宛先である外部受信者の数を示すメールヒントを表示する必要があるかどうかを示します。
ms.openlocfilehash: fc32e5c4a95f0e33b5532af9c77d31bd6446e641
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460471"
---
# <a name="showexternalrecipientcount"></a>Showexternal受信者カウント

**Showexternalrecipients count**要素は、 [getmailtips ヒント操作](getmailtips-operation.md)のコンシューマーが、メッセージの宛先である外部受信者の数を示すメールヒントを表示する必要があるかどうかを示します。 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
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
|[Mailヒント構成 (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |メールヒントサービスのサービス構成情報が保存されています。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、 [Getmailtips ヒント操作](getmailtips-operation.md)のコンシューマーが、メッセージの宛先である外部受信者の数を示すメールヒントを表示する必要がある場合は**true**です。 [Getmailtips ヒント操作](getmailtips-operation.md)のコンシューマーが、メッセージの宛先である外部受信者の数を示すメールヒントを表示する必要がない場合は、値は**false**になります。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetMailTips ヒント操作](getmailtips-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

