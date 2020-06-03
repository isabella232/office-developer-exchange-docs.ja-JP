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
description: Actions 要素は、条件が満たされたときにメッセージに対して実行できる一連のアクションを表します。
ms.openlocfilehash: 2ac53778b583595fa8be07f2c5110a9e2df16eca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465066"
---
# <a name="actions"></a>アクション

**Actions**要素は、条件が満たされたときにメッセージに対して実行できる一連のアクションを表します。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[カテゴリを割り当てる](assigncategories.md) <br/> |電子メールメッセージにスタンプされている分類項目を表します。  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |電子メールアイテムがコピーされるフォルダーの ID を指定します。  <br/> |
|[Delete](delete.md) <br/> |メッセージを [削除済みアイテム] フォルダーに移動するかどうかを示します。  <br/> |
|[ForwardAsAttachmentToRecipients 添付ファイル](forwardasattachmenttorecipients.md) <br/> |添付ファイルとして転送されるメッセージの送信先の電子メールアドレスを示します。  <br/> |
|[Forwardトーラス (Pitor)](forwardtorecipients.md) <br/> |メッセージが転送される電子メールアドレスを示します。  <br/> |
|[マーク (重要)](markimportance.md) <br/> |メッセージに対してスタンプされる重要度を指定します。  <br/> |
|[MarkAsRead](markasread.md) <br/> |メッセージを開封済みとしてマークするかどうかを示します。  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |電子メールアイテムの移動先フォルダーの ID を指定します。  <br/> |
|[PermanentDelete](permanentdelete.md) <br/> |メッセージが完全に削除され、削除済みアイテムフォルダーに保存されないようにするかどうかを示します。  <br/> |
|[RedirectToRecipients](redirecttorecipients.md) <br/> |メッセージがリダイレクトされる電子メールアドレスを示します。  <br/> |
|[SendSMSAlertToRecipients](sendsmsalerttorecipients.md) <br/> |短いメッセージサービス (SMS) の通知が送信される携帯電話の番号を示します。  <br/> |
|[ServerReplyWithMessage](serverreplywithmessage.md) <br/> |を示し. 受信メッセージへの返信として送信されるテンプレートメッセージの ID です。  <br/> |
|[StopProcessingRules](stopprocessingrules.md) <br/> |後続のルールを評価するかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ルール (RuleType)](rule-ruletype.md) <br/> |ユーザーのメールボックス内の1つのルールを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目

- [条件](conditions.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

