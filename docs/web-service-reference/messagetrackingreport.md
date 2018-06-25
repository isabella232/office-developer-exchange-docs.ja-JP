---
title: MessageTrackingReport
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
description: MessageTrackingReport 要素には、GetMessageTrackingReport の操作で返される 1 つのメッセージが含まれています。
ms.openlocfilehash: d01e0fbf099d096c7f255a8e94070e330577e6ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832457"
---
# <a name="messagetrackingreport"></a>MessageTrackingReport

**MessageTrackingReport**要素には、 [GetMessageTrackingReport の操作](getmessagetrackingreport-operation.md)で返される 1 つのメッセージが含まれています。
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[送信者 (EmailAddressType)](sender-emailaddresstype.md) <br/> |電子メール メッセージの送信者の連絡先の情報が含まれています。  <br/> |
|[PurportedSender](purportedsender.md) <br/> |申し立ての送信者の電子メール メッセージの連絡先の情報が含まれています。  <br/> |
|[Subject](subject.md) <br/> |電子メール メッセージの件名が含まれています。  <br/> |
|[SubmitTime](submittime.md) <br/> |電子メール メッセージが送信された時刻が含まれています。  <br/> |
|[OriginalRecipients](originalrecipients.md) <br/> |電子メール メッセージの受信者の一覧が含まれています。  <br/> |
|[RecipientTrackingEvents](recipienttrackingevents.md) <br/> |受信者の 1 つまたは複数の追跡イベントのリストが含まれています。  <br/> |
|[プロパティ (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |1 つまたは複数の追跡のプロパティの一覧が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |1 つの結果が含まれています[GetMessageTrackingReport の操作](getmessagetrackingreport-operation.md)を要求します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)
  
[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
  
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

