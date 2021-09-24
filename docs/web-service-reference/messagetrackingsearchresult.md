---
title: MessageTrackingSearchResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MessageTrackingSearchResult
api_type:
- schema
ms.assetid: 8ea77aa8-b93f-4287-be36-0a9da06e0946
description: MessageTrackingSearchResult 要素には、FindMessageTrackingReportResponse 要素の 1 つのメッセージ結果が含まれる。
ms.openlocfilehash: 2bd70461b2896d0204b163365d525f76d42bb213
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523881"
---
# <a name="messagetrackingsearchresult"></a>MessageTrackingSearchResult

**MessageTrackingSearchResult** 要素には [、FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md)要素の 1 つのメッセージ結果が含まれる。 
  
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
|[件名](subject.md) <br/> |電子メール メッセージの件名が含まれる。  <br/> |
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |電子メール メッセージの送信者のアドレスを含む。  <br/> |
|[PurportedSender](purportedsender.md) <br/> |電子メール メッセージの疑いがある送信者の連絡先情報が含まれる。  <br/> |
|[Recipients (ArrayOfRecipientsType)](recipients-arrayofrecipientstype.md) <br/> |このメッセージを受信した電子メール アドレスの一覧が含まれます。  <br/> |
|[SubmittedTime](submittedtime.md) <br/> |メッセージが送信された時刻を格納します。  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |トランスポート データベース内のメッセージを識別する内部 ID が含まれています。  <br/> |
|[PreviousHopServer](previoushopserver.md) <br/> |メッセージを以前に受け入れ、フォレスト内のサーバーの名前を格納します。  <br/> |
|[FirstHopServer](firsthopserver.md) <br/> |メッセージを最初に受け入れるフォレスト内のサーバーの名前を格納します。  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |1 つ以上の追跡プロパティの一覧が含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageTrackingSearchResults](messagetrackingsearchresults.md) <br/> |検索条件に一致するメッセージの一覧が含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

