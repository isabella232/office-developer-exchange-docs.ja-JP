---
title: Mailヒント構成 (MailTipsServiceConfiguration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsConfiguration
api_type:
- schema
ms.assetid: 9a34515e-815b-4c61-b118-d5f66b80238f
description: Mailヒント構成要素には、メールヒントサービスのサービス構成情報が含まれています。
ms.openlocfilehash: 9128ee99545066899c3b27b624f10a9f1bd36c9d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467789"
---
# <a name="mailtipsconfiguration-mailtipsserviceconfiguration"></a>Mailヒント構成 (MailTipsServiceConfiguration)

**Mailヒント構成**要素には、メールヒントサービスのサービス構成情報が含まれています。 
  
```XML
<MailTipsConfiguration>
   <MailTipsEnabled/>
   <MaxRecipientsPerGetMailTipsRequest/>
   <MaxMessageSize/>
   <LargeAudienceThreshold/>
   <ShowExternalRecipientCount/>
   <InternalDomains/>
</MailTipsConfiguration>
```

 **MailTipsServiceConfiguration**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Mailヒント有効](mailtipsenabled.md) <br/> |メールヒントサービスが利用可能かどうかを示します。 この要素は必須です。  <br/> |
|[Max受信者 Spergetmailヒント要求](maxrecipientspergetmailtipsrequest.md) <br/> |[Getmailtips ヒント操作](getmailtips-operation.md)に渡すことができる受信者の最大数を示します。 この要素は必須です。  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |受信者が受け付けることができる最大メッセージサイズを表します。 この要素は必須です。  <br/> |
|[LargeAudienceThreshold](largeaudiencethreshold.md) <br/> |クライアントの大規模な対象ユーザーのしきい値を表します。 この要素は必須です。  <br/> |
|[Showexternal受信者カウント](showexternalrecipientcount.md) <br/> |[Getmailtips ヒント操作](getmailtips-operation.md)のコンシューマーが、メッセージの宛先である外部受信者の数を示すメールヒントを表示する必要があるかどうかを示します。 この要素は必須です。  <br/> |
|[InternalDomains (SmtpDomainList)](internaldomains-smtpdomainlist.md) <br/> |組織の内部 SMTP ドメインのリストを識別します。 この要素は必須です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |サービス構成の設定が含まれます。  <br/> |
   
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

