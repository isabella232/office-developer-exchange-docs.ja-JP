---
title: PendingMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PendingMailTips
api_type:
- schema
ms.assetid: 0cd70eea-8d36-4b1b-bf80-5edf359e7ba7
description: PendingMailTips 要素は、サーバーの処理タイムアウトが期限切れになる前に、この要素のメール ヒントを評価できないと示します。
ms.openlocfilehash: cadf1839acaeb7c25d1bbf42af5fc866f6c7a4cd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521761"
---
# <a name="pendingmailtips"></a>PendingMailTips

**PendingMailTips 要素** は、サーバーの処理タイムアウトが期限切れになる前に、この要素のメール ヒントを評価できないと示します。 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
```

 **MailTipTypes**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[メールヒント](mailtips.md) <br/> |さまざまな種類のメール ヒントの値を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、PendingMailTips 要素に使用できる値を示** します。 
  
|**値**|**説明**|
|:-----|:-----|
|すべて  <br/> |使用可能なすべてのメール ヒントを表します。  <br/> |
|OutOfOfficeMessage  <br/> |[アウト オブ Office ( OOF) メッセージを表します。  <br/> |
|MailboxFullStatus  <br/> |満たされているメールボックスの状態を表します。  <br/> |
|CustomMailTip  <br/> |カスタム メール ヒントを表します。  <br/> |
|ExternalMemberCount  <br/> |外部メンバーの数を表します。  <br/> |
|TotalMemberCount  <br/> |すべてのメンバーの数を表します。  <br/> |
|MaxMessageSize  <br/> |受信者が受け入れ可能な最大メッセージ サイズを表します。  <br/> |
|DeliveryRestriction  <br/> |配信の制限によって、送信者のメッセージが受信者に届かないかどうかを示します。  <br/> |
|ModerationStatus  <br/> |送信者のメッセージをモデレーターが確認するかどうかを示します。  <br/> |
|InvalidRecipient  <br/> |受信者が無効かどうかを示します。  <br/> |
   
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

