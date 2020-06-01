---
title: FindMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindMessageTrackingReport
api_type:
- schema
ms.assetid: 7ca6e2f7-aae1-4920-b839-73513ba8d4d8
description: FindMessageTrackingReport 要素は、検索するメッセージの種類に関する条件を指定します。
ms.openlocfilehash: d30e5391bb4305cae0004a9788df971a57297cae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462937"
---
# <a name="findmessagetrackingreport"></a>FindMessageTrackingReport

**Findmessagetrackingreport**要素は、検索するメッセージの種類に関する条件を指定します。 
  
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
|[範囲 (非 Emptystringtype)](scope-nonemptystringtype.md) <br/> |メッセージ追跡レポートの詳細を表します。  <br/> |
|[ドメイン (メッセージ追跡)](domain-message-tracking.md) <br/> |メッセージ追跡が実行されるドメインの名前が含まれます。  <br/> |
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |電子メールメッセージの送信者の連絡先情報が保存されています。  <br/> |
|[PurportedSender](purportedsender.md) <br/> |電子メールメッセージの申し立て送信者の連絡先情報が含まれています。  <br/> |
|[[受信者]](recipient.md) <br/> |メッセージの受信者の電子メールアドレスが保存されています。  <br/> |
|[[件名]](subject.md) <br/> |電子メールメッセージの件名を含みます。  <br/> |
|[StartDateTime](startdatetime.md) <br/> |検索の開始日時を格納します。  <br/> |
|[EndDateTime](enddatetime.md) <br/> |検索を終了する日付と時刻を含みます。  <br/> |
|[MessageId](messageid.md) <br/> |検索のメッセージ識別子を含みます。  <br/> |
|[FederatedDeliveryMailbox](federateddeliverymailbox.md) <br/> |クロスプレミスメッセージが送信されたメールボックスの名前が含まれます。  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |診断レポートの詳細レベルを表します。  <br/> |
|[ServerHint](serverhint.md) <br/> |リモートサイトまたはフォレスト内のメッセージを追跡するための開始点を表します。  <br/> |
|[プロパティ (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |1つ以上の追跡プロパティの一覧が含まれています。 この要素は省略できます。  <br/> |
   
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



[FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

