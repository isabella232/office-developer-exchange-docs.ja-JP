---
title: FindMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindMessageTrackingReport
api_type:
- schema
ms.assetid: 7ca6e2f7-aae1-4920-b839-73513ba8d4d8
description: FindMessageTrackingReport 要素は、検索するメッセージの種類の条件を指定します。
ms.openlocfilehash: ec2ab16c6649d85edd86b9438e00ea7cfb9841ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513690"
---
# <a name="findmessagetrackingreport"></a>FindMessageTrackingReport

**FindMessageTrackingReport** 要素は、検索するメッセージの種類の条件を指定します。 
  
```xml
<FindMessageTrackingReport>
   <Scope/>
   <Domain/>
   <Sender/>
   <PurportedSender/>
   <Recipient/>
   <Subject/>
   <StartDateTime/>
   <EndDateTime/>
   <MessageId/>
   <FederatedDeliveryMailbox/>
   <DiagnosticsLevel/>
   <ServerHint/>
   <Properties/>
</FindMessageTrackingReport>
```

 **FindMessageTrackingReportRequestType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Scope (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |メッセージ追跡レポートの広範な機能を表します。  <br/> |
|[Domain (メッセージ追跡)](domain-message-tracking.md) <br/> |メッセージ追跡が実行されるドメインの名前を格納します。  <br/> |
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |電子メール メッセージの送信者の連絡先情報が含まれる。  <br/> |
|[PurportedSender](purportedsender.md) <br/> |電子メール メッセージの疑いがある送信者の連絡先情報が含まれる。  <br/> |
|[[受信者]](recipient.md) <br/> |メッセージの受信者の電子メール アドレスを格納します。  <br/> |
|[件名](subject.md) <br/> |電子メール メッセージの件名が含まれる。  <br/> |
|[StartDateTime](startdatetime.md) <br/> |検索の開始日時を格納します。  <br/> |
|[EndDateTime](enddatetime.md) <br/> |検索の終了日時を格納します。  <br/> |
|[MessageId](messageid.md) <br/> |検索のメッセージ識別子が含まれる。  <br/> |
|[FederatedDeliveryMailbox](federateddeliverymailbox.md) <br/> |クロス前提メッセージが送信されたメールボックスの名前を格納します。  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |診断レポートの詳細レベルを表します。  <br/> |
|[ServerHint](serverhint.md) <br/> |リモート サイトまたはフォレスト内のメッセージを追跡する開始点を表します。  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |1 つ以上の追跡プロパティの一覧が含まれる。 この要素は省略できます。  <br/> |
   
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
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

