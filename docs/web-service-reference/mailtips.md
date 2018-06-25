---
title: メール ヒント
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: メール ヒントの要素は、さまざまな種類のメール ヒントの値を表します。
ms.openlocfilehash: 3a2e95225b09fd2d81db32f821ea3069ab7e7852
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832311"
---
# <a name="mailtips"></a>メール ヒント

**メール ヒント**の要素は、さまざまな種類のメール ヒントの値を表します。 
  
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

 **メール ヒント**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[RecipientAddress](recipientaddress.md) <br/> |受信者のメールボックスを表します。  <br/> |
|[PendingMailTips](pendingmailtips.md) <br/> |サーバーの処理のタイムアウト期間が経過する前にこの要素内のメール ヒントを評価できませんでしたを示します。  <br/> |
|[OutOfOffice](outofoffice.md) <br/> |応答メッセージと応答メッセージを送信するための継続時間を表します。  <br/> |
|[MailboxFull](mailboxfull.md) <br/> |受信者のメールボックスがいっぱいであるかどうかを示します。  <br/> |
|[CustomMailTip](custommailtip.md) <br/> |カスタマイズしたメール ヒントのメッセージを表します。  <br/> |
|[TotalMemberCount](totalmembercount.md) <br/> |グループ内のすべてのメンバーの数を表します。  <br/> |
|[ExternalMemberCount](externalmembercount.md) <br/> |グループ内の外部のメンバーの数を表します。  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |受信者が受け入れることができるメッセージの最大サイズを表します。  <br/> |
|[DeliveryRestricted](deliveryrestricted.md) <br/> |配信の制限が、送信者のメッセージを防ぐため、受信者に到達できないかどうかを示します。  <br/> |
|[IsModerated](ismoderated.md) <br/> |受信者のメールボックスがモデレートされているかどうかを示します。  <br/> |
|[InvalidRecipient (メール ヒント)](invalidrecipient-mailtips.md) <br/> |受信者が有効かどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MailTipsResponseMessageType](mailtipsresponsemessagetype.md) <br/> |メールのヒントの設定を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

