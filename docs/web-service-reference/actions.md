---
title: アクション
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Actions
api_type:
- schema
ms.assetid: c5aa96b1-2d8b-422f-8c2f-f118572ab23f
description: Actions 要素は、条件が満たされた場合にメッセージに対して実行できる一連のアクションを表します。
ms.openlocfilehash: 7f6608af5b8a9eb2772228a638fc42b9558f1e42
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546862"
---
# <a name="actions"></a>アクション

**Actions 要素** は、条件が満たされた場合にメッセージに対して実行できる一連のアクションを表します。 
  
[Rule (RuleType)](rule-ruletype.md)
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AssignCategories](assigncategories.md) <br/> |電子メール メッセージにスタンプされているカテゴリを表します。  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |電子メール アイテムをコピーするフォルダーの ID を識別します。  <br/> |
|[削除](delete.md) <br/> |メッセージを削除済みアイテム フォルダーに移動するかどうかを示します。  <br/> |
|[ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) <br/> |メッセージを添付ファイルとして転送する電子メール アドレスを示します。  <br/> |
|[ForwardToRecipients](forwardtorecipients.md) <br/> |メッセージを転送する電子メール アドレスを示します。  <br/> |
|[MarkImportance](markimportance.md) <br/> |メッセージにスタンプする重要度を指定します。  <br/> |
|[MarkAsRead](markasread.md) <br/> |メッセージを読み取りとしてマークするかどうかを示します。  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |電子メール アイテムを移動するフォルダーの ID を識別します。  <br/> |
|[PermanentDelete](permanentdelete.md) <br/> |メッセージを完全に削除し、削除済みアイテム フォルダーに保存しないかどうかを示します。  <br/> |
|[RedirectToRecipients](redirecttorecipients.md) <br/> |メッセージをリダイレクトする電子メール アドレスを示します。  <br/> |
|[SendSMSAlertToRecipients](sendsmsalerttorecipients.md) <br/> |ショート メッセージ サービス (SMS) アラートを送信する携帯電話番号を示します。  <br/> |
|[ServerReplyWithMessage](serverreplywithmessage.md) <br/> |示します。 受信メッセージへの返信として送信されるテンプレート メッセージの ID。  <br/> |
|[StopProcessingRules](stopprocessingrules.md) <br/> |後続のルールを評価するかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Rule (RuleType)](rule-ruletype.md) <br/> |ユーザーのメールボックス内の 1 つのルールを表します。  <br/> |
   
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

- [条件](conditions.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

