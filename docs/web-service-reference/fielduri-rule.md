---
title: FieldUri (ルール)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: FieldURI 要素は、検証エラーの原因となったルール] フィールドに URI を指定します。
ms.openlocfilehash: 88ba54994625d3a950b58e900f28c986c31eddac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760469"
---
# <a name="fielduri-rule"></a>FieldUri (ルール)

**FieldURI**要素は、検証エラーの原因となったルール] フィールドに URI を指定します。 
  
```XML
<FieldURI/>
```

 **RuleFieldURIType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Error](error.md) <br/> |特定のルールのプロパティの値、述語プロパティの値、またはアクションのプロパティの値の 1 つの検証エラーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、次の文字列のいずれかに制限されています。
  
- 規則 Id
    
- DisplayName
    
- 優先度
    
- IsNotSupported
    
- アクション
    
- 条件のカテゴリ。
    
- 条件: ContainsBodyStrings
    
- 条件: ContainsHeaderStrings
    
- 条件: ContainsRecipientStrings
    
- 条件: ContainsSenderStrings
    
- 条件: ContainsSubjectOrBodyStrings
    
- 条件: ContainsSubjectStrings
    
- 条件: FlaggedForAction
    
- 条件: FromAddresses
    
- 条件: FromConnectedAccounts
    
- 条件: 添付ファイル付き
    
- 条件: 重要性
    
- 条件: IsApprovalRequest
    
- 条件: IsAutomaticForward
    
- 条件: IsAutomaticReply
    
- 条件: 暗号化されたチャレンジ
    
- 条件: IsMeetingRequest
    
- 条件: IsMeetingResponse
    
- 条件: IsNDR
    
- 条件: IsPermissionControlled
    
- 条件: IsReadReceipt
    
- 条件入手します。
    
- 条件: IsVoicemail
    
- 条件: ItemClasses
    
- 条件: MessageClassifications
    
- 条件: NotSentToMe
    
- 条件: SentCcMe
    
- 条件: SentOnlyToMe
    
- 条件: SentToAddresses
    
- 条件: SentToMe
    
- 条件: SentToOrCcMe
    
- 条件: 感度解析
    
- 条件: WithinDateRange
    
- 条件: WithinSizeRange
    
- 例外のカテゴリ。
    
- 例外: ContainsBodyStrings
    
- 例外: ContainsHeaderStrings
    
- 例外: ContainsRecipientStrings
    
- 例外: ContainsSenderStrings
    
- 例外: ContainsSubjectOrBodyStrings
    
- 例外: ContainsSubjectStrings
    
- 例外: FlaggedForAction
    
- 例外: FromAddresses
    
- 例外: FromConnectedAccounts
    
- 例外: 添付ファイル付き
    
- 例外: 重要性
    
- 例外: IsApprovalRequest
    
- 例外: IsAutomaticForward
    
- 例外: IsAutomaticReply
    
- 例外: 暗号化されたチャレンジ
    
- 例外: IsMeetingRequest
    
- 例外: IsMeetingResponse
    
- 例外: IsNDR
    
- 例外: IsPermissionControlled
    
- 例外: IsReadReceipt
    
- 例外: 入手
    
- 例外: IsVoicemail
    
- 例外: ItemClasses
    
- 例外: MessageClassifications
    
- 例外: NotSentToMe
    
- 例外: SentCcMe
    
- 例外: SentOnlyToMe
    
- 例外: SentToAddresses
    
- 例外: SentToMe
    
- 例外: SentToOrCcMe
    
- 例外: 感度解析
    
- 例外: WithinDateRange
    
- 例外: WithinSizeRange
    
- アクション: AssignCategories
    
- アクション: CopyToFolder
    
- アクションの削除:
    
- アクション: ForwardAsAttachmentToRecipients
    
- アクション: ForwardToRecipients
    
- アクション: MarkImportance
    
- アクション: MarkAsRead
    
- アクション: MoveToFolder
    
- アクション: PermanentDelete
    
- アクション: RedirectToRecipients
    
- アクション: SendSMSAlertToRecipients
    
- アクション: ServerReplyWithMessage
    
- アクション: StopProcessingRules
    
- IsEnabled
    
- IsInError
    
- 条件
    
- 例外
    
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

