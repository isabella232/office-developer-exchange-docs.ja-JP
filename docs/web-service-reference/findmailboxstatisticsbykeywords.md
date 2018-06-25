---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: FindMailboxStatisticsByKeywords 要素は、キーワードによってメールボックスの統計情報を検索する要求を指定します。
ms.openlocfilehash: e667f13b66e439dca88d73a5e05d74846183928c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760517"
---
# <a name="findmailboxstatisticsbykeywords"></a>FindMailboxStatisticsByKeywords

**FindMailboxStatisticsByKeywords**要素は、キーワードによってメールボックスの統計情報を検索する要求を指定します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[メールボックス (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) <br/> |保留リストの影響を受けるメールボックスの配列が含まれています。  <br/> |
|[Keywords](keywords-ex15websvcsotherref.md) <br/> |検索のキーワードを指定します。  <br/> |
|[Language](language.md) <br/> |検索クエリで使用する言語が含まれています。  <br/> |
|[送信者](senders.md) <br/> |SMTP アドレスの配列を指定します。  <br/> |
|[受信者 (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |メッセージの受信者の配列を指定します。  <br/> |
|[[開始日](fromdate.md) <br/> |メッセージが送信された日付を指定します。  <br/> |
|[ToDate](todate.md) <br/> |メッセージを受信した日付を指定します。  <br/> |
|[MessageTypes](messagetypes.md) <br/> |検索するメッセージの配列を指定します。  <br/> |
|[SearchDumpster](searchdumpster.md) <br/> |削除済みアイテムを検索するかどうかを指定します。  <br/> |
|[IncludePersonalArchive](includepersonalarchive.md) <br/> |個人用アーカイブを検索に含めるかどうかを指定します。  <br/> |
|[IncludeUnsearchableItems](includeunsearchableitems.md) <br/> |検索できない項目を含めるかどうかを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

