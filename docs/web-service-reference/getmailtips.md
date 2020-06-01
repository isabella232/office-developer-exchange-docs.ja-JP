---
title: GetMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 4a24ff79-f1ae-43a1-9ac2-49baf3eaa173
description: GetMailTips ヒント要素は、取得するメールヒントの受信者と種類を表します。
ms.openlocfilehash: 8ff71ed5d52f713e11188b07c8c93aeee7dfa44d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458636"
---
# <a name="getmailtips"></a>GetMailTips

**Getmailtips**ヒント要素は、取得するメールヒントの受信者と種類を表します。 
  
```XML
<GetMailTips>
   <SendingAs/>
   <Recipients/>
   <MailTipsRequested/>
</GetMailTips>
```

 **Getmailヒント Stype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SendingAs](sendingas.md) <br/> |ユーザーが送信しようとしている電子メールアドレスが含まれています。  <br/> |
|[受信者 (Arrayof受信者 Stype)](recipients-arrayofrecipientstype.md) <br/> |メールのヒントを確認する受信者の一覧が含まれています。  <br/> |
|[Mailヒント要求](mailtipsrequested.md) <br/> |サービスから要求されたメールヒントの種類が含まれます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
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

