---
title: 例外
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
description: 例外要素は、受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を識別します。
ms.openlocfilehash: b875b4dc0029bb9e0bc2bb50c41569fb72ef9268
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760359"
---
# <a name="exceptions"></a>例外

**例外**要素は、受信トレイ ルールの使用可能なルールの例外条件をすべてを表す例外を識別します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Categories](categories-ex15websvcsotherref.md) <br/> |カテゴリ適用する場合の条件または例外の順序で受信したメッセージに適用する必要がありますにはが含まれています。  <br/> |
|[ContainsBodyStrings](containsbodystrings.md) <br/> |適用する場合の条件または例外の順序で受信メッセージの本文に表示する文字列を示します。  <br/> |
|[ContainsHeaderStrings](containsheaderstrings.md) <br/> |Indicaqtes 文字列を適用する場合の条件または例外の順序で受信メッセージのヘッダーに表示する必要があります。  <br/> |
|[ContainsRecipientStrings](containsrecipientstrings.md) <br/> |**ToRecipients**または**CcRecipients**のいずれかの条件または例外を適用する順序で受信メッセージのプロパティに表示される文字列を示します。  <br/> |
|[ContainsSenderStrings](containssenderstrings.md) <br/> |**** プロパティに適用する条件または例外の順序で受信したメッセージに表示する文字列を示します。  <br/> |
|[ContainsSubjectOrBodyStrings](containssubjectorbodystrings.md) <br/> |適用する場合の条件または例外の順序で受信したメッセージの件名または本文に表示する文字列を示します。  <br/> |
|[ContainsSubjectStrings](containssubjectstrings.md) <br/> |適用する場合の条件または例外の順序で受信したメッセージの件名に表示される文字列を示します。  <br/> |
|[FlaggedForAction](flaggedforaction.md) <br/> |適用する場合の条件または例外の順序で受信したメッセージを表示する必要がありますアクションの値のフラグを指定します。  <br/> |
|[FromAddresses](fromaddresses.md) <br/> |元の条件または例外を適用する順序で受信したメッセージを送信する必要がある電子メール アドレスを示します。  <br/> |
|[FromConnectedAccounts](fromconnectedaccounts.md) <br/> |受信メッセージの適用の条件または例外のために集められたを持つ必要がある電子メール アカウントの名前を表します。  <br/> |
|[添付ファイル付き](hasattachments.md) <br/> |受信したメッセージを添付ファイルのある条件または例外を適用する必要があるかどうかを示します。  <br/> |
|[Importance](importance.md) <br/> |適用する場合の条件または例外の順序で受信したメッセージにスタンプする重要性を指定します。  <br/> |
|[IsApprovalRequest](isapprovalrequest.md) <br/> |受信メッセージに適用する条件または例外の順序で要求を承認をする必要があるかどうかを示します。  <br/> |
|[IsAutomaticForward](isautomaticforward.md) <br/> |受信メッセージに適用する条件または例外の順に自動転送をする必要があるかどうかを示します。  <br/> |
|[IsAutomaticReply](isautomaticreply.md) <br/> |受信メッセージに適用する条件または例外の順序で自動返信をする必要があるかどうかを示します。  <br/> |
|[暗号化されたチャレンジ](isencrypted.md) <br/> |受信メッセージが S/MIME 暗号化を適用する場合の条件または例外の順序である必要があるかどうかを示します。  <br/> |
|[IsMeetingRequest](ismeetingrequest.md) <br/> |かどうかメッセージを受信する必要がある会議出席依頼を適用する場合の条件または例外の順序で示します。  <br/> |
|[IsMeetingResponse](ismeetingresponse.md) <br/> |受信メッセージが会議のためには条件や例外条件を適用する返答をする必要があるかどうかを示します。  <br/> |
|[IsNDR](isndr.md) <br/> |適用する場合の条件または例外の順序で受信メッセージが配信不能レポート (Ndr) をする必要があるかどうかを示します。  <br/> |
|[IsPermissionControlled](ispermissioncontrolled.md) <br/> |適用する場合の条件または例外の順序で受信メッセージがアクセス許可の制御 (RMS 保護) をする必要があるかどうかを示します  <br/> |
|[IsReadReceipt](isreadreceipt.md) <br/> |かどうかの受信メッセージ読み取る必要があります適用の条件または例外のために領収書を示します。  <br/> |
|[入手](issigned.md) <br/> |S/MIME の署名を適用する場合の条件または例外の順序で受信したメッセージがある必要があるかどうかを示します。  <br/> |
|[IsVoicemail](isvoicemail.md) <br/> |適用の条件または例外のためにボイス メール メッセージを受信したメッセージがある必要があるかどうかを示します。  <br/> |
|[ItemClasses](itemclasses.md) <br/> |適用する場合の条件または例外の順序で受信したメッセージにスタンプする必要があります項目クラスを表します。  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |メッセージの分類を適用する場合の条件または例外の順序で受信したメッセージにスタンプする必要があることを表します。  <br/> |
|[NotSentToMe](notsenttome.md) <br/> |**ToRecipients**プロパティを適用する場合の条件または例外の順序で受信したメッセージのメールボックスの所有者がある必要がありますいないかどうかを示します。  <br/> |
|[SentCcMe](sentccme.md) <br/> |**CcRecipients**プロパティを適用する場合の条件または例外の順序で受信メッセージのあるメールボックスの所有者があるかどうかを示します。  <br/> |
|[SentOnlyToMe](sentonlytome.md) <br/> |**ToRecipients**プロパティを適用する場合の条件または例外の順序で受信メッセージの 1 つのみを使用するメールボックスの所有者があるかどうかを示します。  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |適用する条件または例外の順序でに送信されている受信メッセージを持つ電子メール アドレスを示します。  <br/> |
|[SentToMe](senttome.md) <br/> |**ToRecipients**プロパティを適用する場合の条件または例外の順序で受信したメッセージのあるメールボックスの所有者があるかどうかを示します。  <br/> |
|[SentToOrCcMe](senttoorccme.md) <br/> |**ToRecipients**または**CcRecipients**のいずれかの条件または例外を適用する順序で受信メッセージのプロパティで、メールボックスの所有者があるかどうかを示します。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |感度を適用する場合の条件または例外の順序で受信したメッセージにスタンプする必要があることを示します。  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |受信したメッセージが適用の条件または例外のために到着した日付の範囲を指定します。  <br/> |
|[WithinSizeRange](withinsizerange.md) <br/> |適用する場合の条件または例外の順序で受信メッセージをする必要のある最小値と最大サイズを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ルール (RuleType)](rule-ruletype.md) <br/> |1 つのルールが含まれていて、ユーザーのメールボックス内のルールを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

ルールの述語は、ルールの条件または例外として使用されます。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[条件](conditions.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

