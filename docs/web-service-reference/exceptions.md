---
title: Exceptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exceptions
api_type:
- schema
ms.assetid: 7cd63ac2-3441-4ed4-915b-6f90af4b28fc
description: Exceptions 要素は、受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を識別します。
ms.openlocfilehash: 1afc2980391ee588f9b9b813b87c2c699de3a6df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463357"
---
# <a name="exceptions"></a>Exceptions

**Exceptions**要素は、受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を識別します。 
  
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
|[Categories](categories-ex15websvcsotherref.md) <br/> |条件または例外を適用するために、受信メッセージに適用する必要があるカテゴリを含みます。  <br/> |
|[大き Body文字列](containsbodystrings.md) <br/> |条件または例外を適用するために、受信メッセージの本文に表示する必要がある文字列を示します。  <br/> |
|[ContainsHeaderStrings](containsheaderstrings.md) <br/> |条件または例外を適用するために、受信メッセージのヘッダーに表示する必要がある文字列を Indicaqtes します。  <br/> |
|[持つ受信者文字列](containsrecipientstrings.md) <br/> |条件または例外を適用するために、受信メッセージの**torな piの**イベントまたは**ccrecipients**各プロパティに表示する必要がある文字列を示します。  <br/> |
|[文字列](containssenderstrings.md) <br/> |条件または例外を適用するために、受信メッセージの**From**プロパティに表示する必要がある文字列を示します。  <br/> |
|[ContainsSubjectOrBodyStrings](containssubjectorbodystrings.md) <br/> |条件または例外を適用するために、受信メッセージの本文または件名のどちらかに表示する必要がある文字列を示します。  <br/> |
|[大き Subjectstrings](containssubjectstrings.md) <br/> |条件または例外を適用するために、受信メッセージの件名に表示する必要がある文字列を示します。  <br/> |
|[FlaggedForAction](flaggedforaction.md) <br/> |条件または例外を適用するために、受信メッセージに表示する必要があるアクション値のフラグを指定します。  <br/> |
|[FromAddresses](fromaddresses.md) <br/> |条件または例外を適用するために、受信メッセージを送信する必要がある電子メールアドレスを示します。  <br/> |
|[FromConnectedAccounts](fromconnectedaccounts.md) <br/> |条件または例外を適用するために、受信メッセージが集計されている必要がある電子メールアカウント名を表します。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |条件または例外を適用するために、受信メッセージに添付ファイルを含める必要があるかどうかを示します。  <br/> |
|[Importance](importance.md) <br/> |条件または例外を適用するために、受信メッセージにスタンプされる重要度を指定します。  <br/> |
|[IsApprovalRequest](isapprovalrequest.md) <br/> |条件または例外を適用するために、受信メッセージが承認要求であるかどうかを示します。  <br/> |
|[Is自動転送](isautomaticforward.md) <br/> |条件または例外を適用するために、受信メッセージを自動転送する必要があるかどうかを示します。  <br/> |
|[Is自動応答](isautomaticreply.md) <br/> |条件または例外を適用するために、受信メッセージが自動応答である必要があるかどうかを示します。  <br/> |
|[IsEncrypted](isencrypted.md) <br/> |条件または例外を適用するために、受信メッセージを S/MIME で暗号化する必要があるかどうかを示します。  <br/> |
|[Is会議要求](ismeetingrequest.md) <br/> |条件または例外を適用するために、受信メッセージが会議出席依頼である必要があるかどうかを示します。  <br/> |
|[Is会議の応答](ismeetingresponse.md) <br/> |条件または例外を適用するために、受信メッセージが会議出席依頼に応答する必要があるかどうかを示します。  <br/> |
|[IsNDR](isndr.md) <br/> |条件または例外を適用するために、受信メッセージが配信不能レポート (Ndr) である必要があるかどうかを示します。  <br/> |
|[IsPermissionControlled](ispermissioncontrolled.md) <br/> |条件または例外を適用するために、受信メッセージが権限制御される (RMS 保護) 必要があるかどうかを示します。  <br/> |
|[IsReadReceipt](isreadreceipt.md) <br/> |条件または例外を適用するために、受信メッセージが開封確認である必要があるかどうかを示します。  <br/> |
|[IsSigned](issigned.md) <br/> |条件または例外を適用するために、受信メッセージが S/MIME で署名されている必要があるかどうかを示します。  <br/> |
|[IsVoicemail メール](isvoicemail.md) <br/> |条件または例外を適用するために、受信メッセージがボイスメールメッセージである必要があるかどうかを示します。  <br/> |
|[ItemClasses](itemclasses.md) <br/> |条件または例外を適用するために、受信メッセージにスタンプする必要があるアイテムクラスを表します。  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |条件または例外を適用するために、受信メッセージにスタンプする必要があるメッセージ分類を表します。  <br/> |
|[NotSentToMe](notsenttome.md) <br/> |条件または例外を適用するために、メールボックスの所有者が受信メッセージの**トーラス**プロパティに含まれないようにする必要があるかどうかを示します。  <br/> |
|[Ccme の説明](sentccme.md) <br/> |条件または例外を適用するために、メールボックスの所有者が受信メッセージの**Ccrecipients**プロパティにある必要があるかどうかを示します。  <br/> |
|[SentOnlyToMe](sentonlytome.md) <br/> |条件または例外を適用するために、メールボックスの所有者が受信メッセージの**Torecipients**プロパティにある唯一の所有者である必要があるかどうかを示します。  <br/> |
|[住所](senttoaddresses.md) <br/> |条件または例外を適用するために、受信メッセージの送信先の電子メールアドレスを指定します。  <br/> |
|[SentToMe](senttome.md) <br/> |条件または例外を適用するために、メールボックスの所有者が受信メッセージの**Torecipients**プロパティにある必要があるかどうかを示します。  <br/> |
|[「Orccme」](senttoorccme.md) <br/> |条件または例外を適用するために、メールボックスの所有者が受信メッセージの**Torecipients**イベントまたは**ccrecipients**プロパティのいずれかに含まれている必要があるかどうかを示します。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |条件または例外を適用するために、受信メッセージにスタンプする必要がある感度を示します。  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |条件または例外を適用するために、受信メッセージが受信される必要がある日付範囲を指定します。  <br/> |
|[WithinSizeRange](withinsizerange.md) <br/> |条件または例外を適用するために、受信メッセージが必要とする最小サイズと最大サイズを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ルール (RuleType)](rule-ruletype.md) <br/> |1つのルールを含み、ユーザーのメールボックス内のルールを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

ルールの述語は、ルールの条件または例外として使用されます。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[条件](conditions.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

