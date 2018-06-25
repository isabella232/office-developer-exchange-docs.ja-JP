---
title: アクション
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Actions
api_type:
- schema
ms.assetid: c5aa96b1-2d8b-422f-8c2f-f118572ab23f
description: アクション要素では、一連の条件が満たされるときに、メッセージに対して実行される利用可能なアクションを表します。
ms.openlocfilehash: 093d2f28135c6077b6cea488591573af0182934b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759272"
---
# <a name="actions"></a>アクション

**アクション**要素では、一連の条件が満たされるときに、メッセージに対して実行される利用可能なアクションを表します。 
  
[ルール (RuleType)](rule-ruletype.md)
  
```XML
<Actions>
    <AssignCategories>
    <CopyToFolder>
    <Delete>
    <ForwardAsAttachmentToRecipients>
    <ForwardToRecipients>
    <MarkImportance>
    <MarkAsRead>
    <MoveToFolder>
    <PermanentDelete>
    <RedirectToRecipients>
    <SendSMSAlertToRecipients>
    <ServerReplyWithMessage>
    <StopProcessingRules>
</Actions>
```

 **RuleActionsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[AssignCategories](assigncategories.md) <br/> |電子メール メッセージにスタンプされているカテゴリを表します。  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |電子メール アイテムをコピーするフォルダーの ID を識別します。  <br/> |
|[Delete](delete.md) <br/> |メッセージを削除済みアイテム フォルダーに移動するかどうかを示します。  <br/> |
|[ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) <br/> |メッセージが添付ファイルとして転送するのには電子メール アドレスを示します。  <br/> |
|[ForwardToRecipients](forwardtorecipients.md) <br/> |メッセージが転送される電子メール アドレスを示します。  <br/> |
|[MarkImportance](markimportance.md) <br/> |メッセージにスタンプするのには重要度を指定します。  <br/> |
|[MarkAsRead](markasread.md) <br/> |メッセージは開封としてマークするかどうかを示します。  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |電子メール アイテムに移動するフォルダーの ID を識別します。  <br/> |
|[PermanentDelete](permanentdelete.md) <br/> |メッセージを完全に削除し、削除済みアイテム フォルダーに保存されないかどうかを示します。  <br/> |
|[RedirectToRecipients](redirecttorecipients.md) <br/> |メッセージがリダイレクトされるように電子メール アドレスを示します。  <br/> |
|[SendSMSAlertToRecipients](sendsmsalerttorecipients.md) <br/> |ショート メッセージ サービス (SMS) アラートが送信するのには携帯電話の番号を示します。  <br/> |
|[ServerReplyWithMessage](serverreplywithmessage.md) <br/> |示します。 受信メッセージへの応答として送信するのには、テンプレートのメッセージの ID です。  <br/> |
|[StopProcessingRules](stopprocessingrules.md) <br/> |後のルールが評価されるかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ルール (RuleType)](rule-ruletype.md) <br/> |ユーザーのメールボックス内の 1 つのルールを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目

- [条件](conditions.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

