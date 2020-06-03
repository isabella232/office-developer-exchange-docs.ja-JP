---
title: および search-messagetrackingreport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReport
api_type:
- schema
ms.assetid: 2740bcf6-f86d-4756-a0f2-24ed6e9b75f7
description: MessageTrackingReport 要素には、GetMessageTrackingReport 操作で返される1つのメッセージが含まれています。
ms.openlocfilehash: fc3e56fbb1bee411fa31751f558f520874133076
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463217"
---
# <a name="messagetrackingreport"></a>および search-messagetrackingreport

**Messagetrackingreport**要素には、 [getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)で返される1つのメッセージが含まれています。
  
```XML
<MessageTrackingReport>
   <Sender/>
   <PurportedSender/>
   <Subject/>
   <SubmitTime/>
   <OriginalRecipients/>
   <RecipientTrackingEvents/>
   <Properties/>
</MessageTrackingReport>
```

 **MessageTrackingReportType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |電子メールメッセージの送信者の連絡先情報が保存されています。  <br/> |
|[PurportedSender](purportedsender.md) <br/> |電子メールメッセージの申し立て送信者の連絡先情報が含まれています。  <br/> |
|[件名](subject.md) <br/> |電子メールメッセージの件名を含みます。  <br/> |
|[SubmitTime](submittime.md) <br/> |電子メールメッセージが送信された時刻を格納します。  <br/> |
|[OriginalRecipients](originalrecipients.md) <br/> |電子メールメッセージの受信者のリストが保存されています。  <br/> |
|[受信者 Trackingevents](recipienttrackingevents.md) <br/> |受信者の1つまたは複数の追跡イベントのリストを含みます。  <br/> |
|[プロパティ (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |1つ以上の追跡プロパティの一覧が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |1つの[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)要求の結果が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)
  
[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
  
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

