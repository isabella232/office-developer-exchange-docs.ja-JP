---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: FindMailboxStatisticsByKeywords 要素は、キーワードによってメールボックス統計情報を検索する要求を指定します。
ms.openlocfilehash: e22c7d8dc849d3fd45d6cb158030cbd82119437e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462529"
---
# <a name="findmailboxstatisticsbykeywords"></a>FindMailboxStatisticsByKeywords

**FindMailboxStatisticsByKeywords**要素は、キーワードによってメールボックス統計情報を検索する要求を指定します。 
  
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
|[メールボックス (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) <br/> |保留の影響を受けるメールボックスの配列を格納します。  <br/> |
|[Keywords](keywords-ex15websvcsotherref.md) <br/> |検索のキーワードを指定します。  <br/> |
|[Language](language.md) <br/> |検索クエリに使用する言語が含まれています。  <br/> |
|[[Senders (送信者)](senders.md)] <br/> |SMTP アドレスの配列を指定します。  <br/> |
|[受信者 (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |メッセージの受信者の配列を指定します。  <br/> |
|[FromDate](fromdate.md) <br/> |メッセージが送信された日付を指定します。  <br/> |
|[半年](todate.md) <br/> |メッセージが受信された日付を指定します。  <br/> |
|[MessageTypes](messagetypes.md) <br/> |検索するメッセージの配列を指定します。  <br/> |
|[SearchDumpster](searchdumpster.md) <br/> |削除済みアイテムを検索するかどうかを指定します。  <br/> |
|[Includeパーソナルアーカイブ](includepersonalarchive.md) <br/> |検索に個人用アーカイブを含めるかどうかを指定します。  <br/> |
|[Include非 Searchableitems](includeunsearchableitems.md) <br/> |検索できないアイテムを含めるかどうかを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

