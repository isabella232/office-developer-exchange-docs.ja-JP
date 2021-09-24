---
title: FieldUri (Rule)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: FieldURI 要素は、検証エラーの原因となるルール フィールドの URI を指定します。
ms.openlocfilehash: c1390f6643614216fa86053368ba012cd0883ff7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513732"
---
# <a name="fielduri-rule"></a>FieldUri (Rule)

**FieldURI 要素** は、検証エラーの原因となるルール フィールドの URI を指定します。 
  
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
|[エラー](error.md) <br/> |特定のルール プロパティ値、述語プロパティ値、またはアクション プロパティ値に対する 1 つの検証エラーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、次のいずれかの文字列に制限されます。
  
- RuleId
    
- DisplayName
    
- 優先度
    
- IsNotSupported
    
- アクション
    
- Condition:Categories
    
- Condition:ContainsBodyStrings
    
- Condition:ContainsHeaderStrings
    
- Condition:ContainsRecipientStrings
    
- Condition:ContainsSenderStrings
    
- Condition:ContainsSubjectOrBodyStrings
    
- Condition:ContainsSubjectStrings
    
- Condition:FlaggedForAction
    
- Condition:FromAddresses
    
- Condition:FromConnectedAccounts
    
- Condition:HasAttachments
    
- Condition:Importance
    
- Condition:IsApprovalRequest
    
- Condition:IsAutomaticForward
    
- Condition:IsAutomaticReply
    
- Condition:IsEncrypted
    
- Condition:IsMeetingRequest
    
- Condition:IsMeetingResponse
    
- Condition:IsNDR
    
- Condition:IsPermissionControlled
    
- Condition:IsReadReceipt
    
- Condition:IsSigned
    
- Condition:IsVoicemail
    
- Condition:ItemClasses
    
- Condition:MessageClassifications
    
- Condition:NotSentToMe
    
- Condition:SentCcMe
    
- Condition:SentOnlyToMe
    
- Condition:SentToAddresses
    
- Condition:SentToMe
    
- Condition:SentToOrCcMe
    
- Condition:Sensitivity
    
- Condition:WithinDateRange
    
- Condition:WithinSizeRange
    
- 例外:カテゴリ
    
- Exception:ContainsBodyStrings
    
- Exception:ContainsHeaderStrings
    
- Exception:ContainsRecipientStrings
    
- Exception:ContainsSenderStrings
    
- Exception:ContainsSubjectOrBodyStrings
    
- Exception:ContainsSubjectStrings
    
- Exception:FlaggedForAction
    
- 例外:FromAddresses
    
- Exception:FromConnectedAccounts
    
- Exception:HasAttachments
    
- 例外:重要度
    
- Exception:IsApprovalRequest
    
- Exception:IsAutomaticForward
    
- Exception:IsAutomaticReply
    
- Exception:IsEncrypted
    
- Exception:IsMeetingRequest
    
- Exception:IsMeetingResponse
    
- Exception:IsNDR
    
- Exception:IsPermissionControlled
    
- Exception:IsReadReceipt
    
- Exception:IsSigned
    
- Exception:IsVoicemail
    
- Exception:ItemClasses
    
- Exception:MessageClassifications
    
- Exception:NotSentToMe
    
- Exception:SentCcMe
    
- Exception:SentOnlyToMe
    
- 例外:SentToAddresses
    
- Exception:SentToMe
    
- Exception:SentToOrCcMe
    
- Exception:Sensitivity
    
- Exception:WithinDateRange
    
- Exception:WithinSizeRange
    
- Action:AssignCategories
    
- Action:CopyToFolder
    
- Action:Delete
    
- Action:ForwardAsAttachmentToRecipients
    
- Action:ForwardToRecipients
    
- Action:MarkImportance
    
- Action:MarkAsRead
    
- Action:MoveToFolder
    
- Action:PermanentDelete
    
- Action:RedirectToRecipients
    
- Action:SendSMSAlertToRecipients
    
- Action:ServerReplyWithMessage
    
- Action:StopProcessingRules
    
- IsEnabled
    
- IsInError
    
- 条件
    
- 例外
    
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

