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
description: MessageTrackingSearchResult 要素には、FindMessageTrackingReportResponse 要素の 1 つのメッセージの結果が含まれています。
ms.openlocfilehash: ad4fb9d9e2266222303bd2015a7afba0bb46721b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832460"
---
# <a name="messagetrackingsearchresult"></a>MessageTrackingSearchResult

**MessageTrackingSearchResult**要素には、 [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md)要素の 1 つのメッセージの結果が含まれています。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Subject](subject.md) <br/> |電子メール メッセージの件名が含まれています。  <br/> |
|[送信者 (EmailAddressType)](sender-emailaddresstype.md) <br/> |電子メール メッセージの送信者のアドレスが含まれています。  <br/> |
|[PurportedSender](purportedsender.md) <br/> |申し立ての送信者の電子メール メッセージの連絡先の情報が含まれています。  <br/> |
|[受信者 (ArrayOfRecipientsType)](recipients-arrayofrecipientstype.md) <br/> |このメッセージを受信した電子メール アドレスの一覧が含まれています。  <br/> |
|[SubmittedTime](submittedtime.md) <br/> |メッセージが送信された時刻が含まれています。  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |トランスポート データベースのメッセージを識別する内部の ID が含まれています。  <br/> |
|[PreviousHopServer](previoushopserver.md) <br/> |以前のメッセージを承諾するフォレスト内のサーバーの名前が含まれています。  <br/> |
|[FirstHopServer](firsthopserver.md) <br/> |フォレスト内の最初のメッセージを受け付けでサーバーの名前が含まれています。  <br/> |
|[プロパティ (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |1 つまたは複数の追跡のプロパティの一覧が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageTrackingSearchResults](messagetrackingsearchresults.md) <br/> |検索条件に一致するメッセージの一覧が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

