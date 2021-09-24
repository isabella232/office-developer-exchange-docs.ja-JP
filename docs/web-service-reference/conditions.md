---
title: 条件
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Conditions
api_type:
- schema
ms.assetid: f049a48c-9585-43f7-8549-0b8cb19a5eea
description: Conditions 要素は、満たされるとルールのルール アクションをトリガーする条件を識別します。
ms.openlocfilehash: 55e569c2aa393c79eb4e712711fb2e7b4107023b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515979"
---
# <a name="conditions"></a>条件

**Conditions 要素** は、満たされるとルールのルール アクションをトリガーする条件を識別します。 
  
```XML
<Conditions>
   <Categories/>
   <ContainsBodyStrings/>
   <ContainsHeaderStrings/>
   <ContainsRecipientStrings/>
   <ContainsSenderStrings/>
   <ContainsSubjectOrBodyStrings/>
   <ContainsSubjectStrings/>
   <FlaggedForAction/>
   <FromAddresses/>
   <FromConnectedAccounts/>
   <HasAttachments/>
   <Importance/>
   <IsApprovalRequest/>
   <IsAutomaticForward/>
   <IsAutomaticReply/>
   <IsEncrypted/>
   <IsMeetingRequest/>
   <IsMeetingResponse/>
   <IsNDR/>
   <IsPermissionControlled/>
   <IsReadReceipt/>
   <IsSigned/>
   <IsVoicemail/>
   <ItemClasses/>
   <MessageClassifications/>
   <NotSentToMe/>
   <SentCcMe/>
   <SentOnlyToMe/>
   <SentToAddresses/>
   <SentToMe/>
   <SentToOrCcMe/>
   <Sensitivity/>
   <WithinDateRange/>
   <WithinSizeRange/>
</Conditions>
```

 **RulePredicatesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Categories](categories-ex15websvcsotherref.md) <br/> |条件または例外を適用するために受信メッセージに適用する必要があるカテゴリが含まれます。  <br/> |
|[ContainsBodyStrings](containsbodystrings.md) <br/> |条件または例外を適用するために、受信メッセージの本文に表示する必要がある文字列を示します。  <br/> |
|[ContainsHeaderStrings](containsheaderstrings.md) <br/> |条件または例外を適用するために、受信メッセージのヘッダーに表示する必要がある文字列を示します。  <br/> |
|[ContainsRecipientStrings](containsrecipientstrings.md) <br/> |条件または例外を適用するために、受信メッセージの **ToRecipients** プロパティまたは **CcRecipients** プロパティに表示する必要がある文字列を示します。  <br/> |
|[ContainsSenderStrings](containssenderstrings.md) <br/> |条件または例外を適用するために、受信メッセージの **From** プロパティに表示する必要がある文字列を示します。  <br/> |
|[ContainsSubjectOrBodyStrings](containssubjectorbodystrings.md) <br/> |条件または例外を適用するために、受信メッセージの本文または件名に表示する必要がある文字列を示します。  <br/> |
|[ContainsSubjectStrings](containssubjectstrings.md) <br/> |条件または例外を適用するために受信メッセージの件名に表示する必要がある文字列を示します。  <br/> |
|[FlaggedForAction](flaggedforaction.md) <br/> |条件または例外を適用するために受信メッセージに表示する必要があるアクション値のフラグを指定します。  <br/> |
|[FromAddresses](fromaddresses.md) <br/> |条件または例外を適用するために受信メッセージを送信する必要がある電子メール アドレスを示します。  <br/> |
|[FromConnectedAccounts](fromconnectedaccounts.md) <br/> |条件または例外を適用するために受信メッセージを集約する必要がある電子メール アカウント名を表します。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |条件または例外を適用するために受信メッセージに添付ファイルが必要かどうかを示します。  <br/> |
|[Importance](importance.md) <br/> |条件または例外を適用するために受信メッセージにスタンプされる重要度を指定します。  <br/> |
|[IsApprovalRequest](isapprovalrequest.md) <br/> |条件または例外を適用するために、受信メッセージが承認要求である必要があるかどうかを示します。  <br/> |
|[IsAutomaticForward](isautomaticforward.md) <br/> |条件または例外を適用するために、受信メッセージを自動転送する必要があるかどうかを示します。  <br/> |
|[IsAutomaticReply](isautomaticreply.md) <br/> |条件または例外を適用するために、受信メッセージを自動返信する必要があるかどうかを示します。  <br/> |
|[IsEncrypted](isencrypted.md) <br/> |条件または例外を適用するために、受信メッセージを S/MIME で暗号化する必要があるかどうかを示します。  <br/> |
|[IsMeetingRequest](ismeetingrequest.md) <br/> |条件または例外を適用するために、受信メッセージが会議出席依頼である必要があるかどうかを示します。  <br/> |
|[IsMeetingResponse](ismeetingresponse.md) <br/> |条件または例外を適用するために、受信メッセージが応答を満たしている必要があるかどうかを示します。  <br/> |
|[IsNDR](isndr.md) <br/> |条件または例外を適用するために、受信メッセージが配信不可レポート (NDRs) である必要があるかどうかを示します。  <br/> |
|[IsPermissionControlled](ispermissioncontrolled.md) <br/> |条件または例外を適用するために、受信メッセージをアクセス許可制御 (RMS で保護) する必要があるかどうかを示します。  <br/> |
|[IsReadReceipt](isreadreceipt.md) <br/> |条件または例外を適用するために受信メッセージを読み取る必要があるかどうかを示します。  <br/> |
|[IsSigned](issigned.md) <br/> |条件または例外を適用するために、受信メッセージに S/MIME 署名が必要かどうかを示します。  <br/> |
|[IsVoicemail](isvoicemail.md) <br/> |条件または例外を適用するために、受信メッセージがボイス メール メッセージである必要があるかどうかを示します。  <br/> |
|[ItemClasses](itemclasses.md) <br/> |条件または例外を適用するために受信メッセージにスタンプする必要があるアイテム クラスを表します。  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |条件または例外を適用するために受信メッセージにスタンプする必要があるメッセージの分類を表します。  <br/> |
|[NotSentToMe](notsenttome.md) <br/> |メールボックスの所有者が、条件または例外を適用するために受信メッセージの **ToRecipients** プロパティに含めずにいなければならないかどうかを示します。  <br/> |
|[SentCcMe](sentccme.md) <br/> |メールボックスの所有者が、条件または例外を適用するために受信メッセージの **CcRecipients** プロパティに含む必要があるかどうかを示します。  <br/> |
|[SentOnlyToMe](sentonlytome.md) <br/> |条件または例外を適用するために、受信メッセージの **ToRecipients** プロパティでメールボックスの所有者だけが必要かどうかを示します。  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |条件または例外を適用するために、受信メッセージが送信される必要がある電子メール アドレスを示します。  <br/> |
|[SentToMe](senttome.md) <br/> |メールボックスの所有者が、条件または例外を適用するために受信メッセージの **ToRecipients** プロパティに含む必要があるかどうかを示します。  <br/> |
|[SentToOrCcMe](senttoorccme.md) <br/> |メールボックスの所有者が、条件または例外を適用するために受信メッセージの **ToRecipients** プロパティまたは **CcRecipients** プロパティに含む必要があるかどうかを示します。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |条件または例外を適用するために、受信メッセージにスタンプする必要がある感度を示します。  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |条件または例外を適用するために受信メッセージを受信する必要がある日付範囲を指定します。  <br/> |
|[WithinSizeRange](withinsizerange.md) <br/> |条件または例外を適用するために受信メッセージが必要な最小サイズと最大サイズを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Rule (RuleType)](rule-ruletype.md) <br/> |1 つのルールを含み、ユーザーのメールボックス内のルールを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[例外](exceptions.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

