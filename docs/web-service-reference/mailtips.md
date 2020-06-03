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
description: メールヒント要素は、さまざまな種類のメールヒントの値を表します。
ms.openlocfilehash: 9bacdea7b4f3108f700ed102025445e01a73e69d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44447597"
---
# <a name="mailtips"></a>メール ヒント

メール**ヒント要素は**、さまざまな種類のメールヒントの値を表します。 
  
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
|[PendingMailTips ヒント](pendingmailtips.md) <br/> |この要素のメールヒントが、サーバーの処理タイムアウトが経過する前に評価されなかったことを示します。  <br/> |
|[不在](outofoffice.md) <br/> |応答メッセージと、応答メッセージを送信する時間を表します。  <br/> |
|[MailboxFull](mailboxfull.md) <br/> |受信者のメールボックスがいっぱいになっているかどうかを示します。  <br/> |
|[CustomMailTip](custommailtip.md) <br/> |カスタマイズされたメールヒントメッセージを表します。  <br/> |
|[TotalMemberCount](totalmembercount.md) <br/> |グループ内のすべてのメンバーの数を表します。  <br/> |
|[ExternalMemberCount](externalmembercount.md) <br/> |グループ内の外部メンバーの数を表します。  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |受信者が受け付けることができる最大メッセージサイズを表します。  <br/> |
|[DeliveryRestricted](deliveryrestricted.md) <br/> |配信の制限によって、送信者のメッセージが受信者に届かないようにするかどうかを示します。  <br/> |
|[IsModerated](ismoderated.md) <br/> |受信者のメールボックスがモデレートされているかどうかを示します。  <br/> |
|[InvalidRecipient (メールヒント)](invalidrecipient-mailtips.md) <br/> |受信者が無効かどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Mailヒント Responsemessagetype](mailtipsresponsemessagetype.md) <br/> |メールヒントの設定を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

