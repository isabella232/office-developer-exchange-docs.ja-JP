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
description: FindMessageTrackingReport 要素は、検索するメッセージの種類の条件を指定します。
ms.openlocfilehash: 77545121aa056992248c045af3f3d36566678b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760526"
---
# <a name="findmessagetrackingreport"></a>FindMessageTrackingReport

**FindMessageTrackingReport**要素は、検索するメッセージの種類の条件を指定します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[スコープ (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |どの広範なメッセージのレポートを追跡する必要がありますを表します。  <br/> |
|[ドメイン (メッセージの追跡)](domain-message-tracking.md) <br/> |メッセージ追跡が実行されるドメインの名前が含まれています。  <br/> |
|[送信者 (EmailAddressType)](sender-emailaddresstype.md) <br/> |電子メール メッセージの送信者の連絡先の情報が含まれています。  <br/> |
|[PurportedSender](purportedsender.md) <br/> |申し立ての送信者の電子メール メッセージの連絡先の情報が含まれています。  <br/> |
|[Recipient](recipient.md) <br/> |メッセージの受信者の電子メール アドレスが含まれています。  <br/> |
|[Subject](subject.md) <br/> |電子メール メッセージの件名が含まれています。  <br/> |
|[StartDateTime](startdatetime.md) <br/> |開始の日付と時刻の検索が含まれています。  <br/> |
|[EndDateTime](enddatetime.md) <br/> |終了の日付と時刻の検索が含まれています。  <br/> |
|[メッセージ Id](messageid.md) <br/> |検索対象のメッセージの識別子が含まれています。  <br/> |
|[FederatedDeliveryMailbox](federateddeliverymailbox.md) <br/> |設置型の間のメッセージが送信されたメールボックスの名前が含まれています。  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |診断レポートの詳細のレベルを表します。  <br/> |
|[ServerHint](serverhint.md) <br/> |リモート ・ サイトまたはフォレスト内のメッセージを追跡するための開始点を表します。  <br/> |
|[プロパティ (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |1 つまたは複数の追跡のプロパティの一覧が含まれています。 この要素はオプションです。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
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



[FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

