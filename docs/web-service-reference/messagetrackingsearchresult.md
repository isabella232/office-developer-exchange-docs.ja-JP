---
title: MessageTrackingSearchResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingSearchResult
api_type:
- schema
ms.assetid: 8ea77aa8-b93f-4287-be36-0a9da06e0946
description: MessageTrackingSearchResult 要素には、FindMessageTrackingReportResponse 要素の単一のメッセージの結果が含まれています。
ms.openlocfilehash: 27e70cd9e11b480ab6bbb9b28275f142da7c76ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466683"
---
# <a name="messagetrackingsearchresult"></a>MessageTrackingSearchResult

**MessageTrackingSearchResult**要素には、 [Findmessagetrackingreportresponse](findmessagetrackingreportresponse.md)要素の単一のメッセージの結果が含まれています。 
  
```xml
<MessageTrackingSearchResult>
   <Subject/>
   <Sender/>
   <PurportedSender/>
   <Recipients/>
   <SubmittedTime/>
   <MessageTrackingReportId/>
   <PreviousHopServer/>
   <FirstHopServer/>
   <Properties/>
</MessageTrackingSearchResult>
```

 **FindMessageTrackingSearchResultType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[件名](subject.md) <br/> |電子メールメッセージの件名を含みます。  <br/> |
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |電子メールメッセージの送信者のアドレスを含みます。  <br/> |
|[PurportedSender](purportedsender.md) <br/> |電子メールメッセージの申し立て送信者の連絡先情報が含まれています。  <br/> |
|[受信者 (Arrayof受信者 Stype)](recipients-arrayofrecipientstype.md) <br/> |このメッセージを受信した電子メールアドレスの一覧が含まれています。  <br/> |
|[SubmittedTime](submittedtime.md) <br/> |メッセージが送信された日時が含まれます。  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |トランスポートデータベース内のメッセージを識別する内部 ID を格納します。  <br/> |
|[PreviousHopServer](previoushopserver.md) <br/> |以前にメッセージを受諾したフォレスト内のサーバーの名前が含まれます。  <br/> |
|[FirstHopServer](firsthopserver.md) <br/> |最初にメッセージを受け入れたフォレスト内のサーバーの名前が含まれます。  <br/> |
|[プロパティ (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |1つ以上の追跡プロパティの一覧が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageTrackingSearchResults](messagetrackingsearchresults.md) <br/> |検索条件に一致するメッセージの一覧が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

