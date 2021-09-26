---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: FindMailboxStatisticsByKeywords 要素は、キーワードによってメールボックスの統計情報を検索する要求を指定します。
ms.openlocfilehash: 3f84b0c3bb2a4a0a2a164b9e9120c3505073417e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546505"
---
# <a name="findmailboxstatisticsbykeywords"></a>FindMailboxStatisticsByKeywords

**FindMailboxStatisticsByKeywords** 要素は、キーワードによってメールボックスの統計情報を検索する要求を指定します。 
  
```XML
<FindMailboxStatisticsByKeywords>
    <Mailboxes/>
    <Keywords/>
    <Language/>
    <Senders/>
    <Recipients/>
    <FromDate/>
    <ToDate/>
    <MessageTypes/>
    <SearchDumpster/>
    <IncludePersonalArchive/>
    <IncludeUnsearchableItems/>
</FindMailboxStatisticsByKeywords>
```

 **FindMailboxStatisticsByKeywordsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Mailboxes (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) <br/> |保留の影響を受けるメールボックスの配列を格納します。  <br/> |
|[Keywords](keywords-ex15websvcsotherref.md) <br/> |検索のキーワードを指定します。  <br/> |
|[Language](language.md) <br/> |検索クエリに使用される言語が含まれる。  <br/> |
|[[Senders (送信者)](senders.md)] <br/> |SMTP アドレスの配列を指定します。  <br/> |
|[Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |メッセージの受信者の配列を指定します。  <br/> |
|[FromDate](fromdate.md) <br/> |メッセージが送信された日付を指定します。  <br/> |
|[ToDate](todate.md) <br/> |メッセージが受信された日付を指定します。  <br/> |
|[MessageTypes](messagetypes.md) <br/> |検索するメッセージの配列を指定します。  <br/> |
|[SearchDumpster](searchdumpster.md) <br/> |削除済みアイテムを検索するかどうかを指定します。  <br/> |
|[IncludePersonalArchive](includepersonalarchive.md) <br/> |個人用アーカイブを検索に含めるかどうかを指定します。  <br/> |
|[IncludeUnsearchableItems](includeunsearchableitems.md) <br/> |検索できないアイテムを含めるかどうかを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

