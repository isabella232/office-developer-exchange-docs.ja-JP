---
title: メール ヒント
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: MailTips 要素は、さまざまな種類のメール ヒントの値を表します。
ms.openlocfilehash: bf7ed542d51f2a8cb3172275be12cb72104bc5b2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511139"
---
# <a name="mailtips"></a>メール ヒント

**MailTips 要素は**、さまざまな種類のメール ヒントの値を表します。 
  
```XML
<MailTips>
   <RecipientAddress/>
   <PendingMailTips/>
   <OutOfOffice/>
   <MailboxFull/>
   <CustomMailTip/>
   <TotalMemberCount/>
   <ExternalMemberCount/>
   <MaxMessageSize/>
   <DeliveryRestricted/>
   <IsModerated/>
   <InvalidRecipient/>
</MailTips>
```

 **メールヒント**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[RecipientAddress](recipientaddress.md) <br/> |受信者のメールボックスを表します。  <br/> |
|[PendingMailTips](pendingmailtips.md) <br/> |サーバーの処理タイムアウトが期限切れになる前に、この要素のメール ヒントを評価できないかどうかを示します。  <br/> |
|[OutOfOffice](outofoffice.md) <br/> |応答メッセージと、応答メッセージを送信する期間を表します。  <br/> |
|[MailboxFull](mailboxfull.md) <br/> |受信者のメールボックスが満たされているかどうかを示します。  <br/> |
|[CustomMailTip](custommailtip.md) <br/> |カスタマイズされたメール ヒント メッセージを表します。  <br/> |
|[TotalMemberCount](totalmembercount.md) <br/> |グループ内のすべてのメンバーの数を表します。  <br/> |
|[ExternalMemberCount](externalmembercount.md) <br/> |グループ内の外部メンバーの数を表します。  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |受信者が受け入れ可能な最大メッセージ サイズを表します。  <br/> |
|[DeliveryRestricted](deliveryrestricted.md) <br/> |配信の制限によって、送信者のメッセージが受信者に届かないかどうかを示します。  <br/> |
|[IsModerated](ismoderated.md) <br/> |受信者のメールボックスがモデ管理されているかどうかを示します。  <br/> |
|[InvalidRecipient (MailTips)](invalidrecipient-mailtips.md) <br/> |受信者が無効かどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MailTipsResponseMessageType](mailtipsresponsemessagetype.md) <br/> |メール ヒントの設定を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

