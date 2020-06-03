---
title: FieldUri (ルール)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: FieldURI 要素は、検証エラーの原因となったルールフィールドへの URI を指定します。
ms.openlocfilehash: 3d88efdf951af580f81b5e2e7a544dcdf70ea830
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461248"
---
# <a name="fielduri-rule"></a>FieldUri (ルール)

**FieldURI**要素は、検証エラーの原因となったルールフィールドへの URI を指定します。 
  
```XML
<FieldURI/>
```

 **RuleFieldURIType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Error](error.md) <br/> |特定のルールプロパティ値、述語プロパティ値、または action プロパティ値に対する1つの検証エラーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、次の文字列のいずれかに制限されています。
  
- RuleId
    
- DisplayName
    
- 優先度
    
- IsNotSupported
    
- アクション
    
- 条件: カテゴリ
    
- 条件: 文字列
    
- 条件: ContainsHeaderStrings
    
- 条件: 次の文字列を持つ
    
- 条件: という文字列
    
- 条件: ContainsSubjectOrBodyStrings
    
- 条件: 大き Subjectstrings
    
- 条件: FlaggedForAction
    
- 条件: FromAddresses
    
- 条件: FromConnectedAccounts
    
- 条件: HasAttachments
    
- 条件: 重要度
    
- 条件: IsApprovalRequest
    
- 条件: Is自動転送
    
- 条件: Is自動応答
    
- 条件: IsEncrypted
    
- 条件: Is会議要求
    
- 条件: Is会議応答
    
- 条件: IsNDR
    
- 条件: IsPermissionControlled
    
- 条件: IsReadReceipt
    
- 条件: IsSigned
    
- 条件: IsVoicemail メール
    
- 条件: ItemClasses
    
- 条件: MessageClassifications
    
- 条件: NotSentToMe
    
- 条件: [Ccme]
    
- 条件: SentOnlyToMe
    
- 条件: 文のアドレス
    
- 条件: SentToMe
    
- 条件: 説明文
    
- 条件: 秘密度
    
- 条件: WithinDateRange
    
- 条件: WithinSizeRange
    
- 例外: カテゴリ
    
- 例外: 次の文字列があります。
    
- 例外: ContainsHeaderStrings
    
- 例外: すべての受信者文字列
    
- 例外: という文字列
    
- 例外: ContainsSubjectOrBodyStrings
    
- 例外: 大き Subjectstrings
    
- 例外: FlaggedForAction
    
- 例外: FromAddresses
    
- 例外: FromConnectedAccounts
    
- 例外: HasAttachments
    
- 例外: 重要度
    
- 例外: IsApprovalRequest
    
- 例外: Is自動転送
    
- 例外: Is自動応答
    
- 例外: IsEncrypted
    
- 例外: Is会議要求
    
- 例外: Is会議応答
    
- 例外: IsNDR
    
- 例外: IsPermissionControlled
    
- 例外: IsReadReceipt
    
- 例外: IsSigned
    
- 例外: IsVoicemail メール
    
- 例外: ItemClasses
    
- 例外: MessageClassifications
    
- 例外: NotSentToMe
    
- 例外: [Ccme]
    
- 例外: SentOnlyToMe
    
- 例外: アドレスの説明
    
- 例外: SentToMe
    
- 例外: 文の説明
    
- 例外: 秘密度
    
- 例外: WithinDateRange
    
- 例外: WithinSizeRange
    
- アクション: カテゴリを割り当てる
    
- アクション: CopyToFolder
    
- アクション: 削除
    
- アクション: forwardasattachmenttorattachmentpiattachment
    
- アクション: forwardtorpipipi
    
- アクション: マーク (重要)
    
- アクション: MarkAsRead
    
- アクション: MoveToFolder
    
- アクション: PermanentDelete
    
- アクション: Redirecttorの Piん
    
- アクション: SendSMSAlertToRecipients
    
- アクション: ServerReplyWithMessage
    
- アクション: StopProcessingRules
    
- IsEnabled
    
- IsInError
    
- 条件
    
- Exceptions
    
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

