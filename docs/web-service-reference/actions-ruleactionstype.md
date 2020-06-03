---
title: Actions (RuleActionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2afba70c-65f7-458c-a4e6-a2cd9bccc0f9
description: Actions 要素には、受信トレイルールに関連付けられたアクションのリストが含まれています。
ms.openlocfilehash: fbef3b69b1688d7c612af018d6a19f9ec1728066
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529680"
---
# <a name="actions-ruleactionstype"></a>Actions (RuleActionsType)

**Actions**要素には、受信トレイルールに関連付けられたアクションのリストが含まれています。 
  
```XML
<Actions>
   <AssignCategories/>
   <CopyToFolder/>
   <Delete/>
   <ForwardAsAttachmentToRecipients/>
   <ForwardToRecipients/>
   <MarkImportance/>
   <MarkAsRead/>
   <MoveToFolder/>
   <PermanentDelete/>
   <RedirectToRecipients/>
   <SendSMSAlertToRecipients/>
   <ServerReplyWithMessage/>
   <StopProcessingRules/>
</Actions>
```

 **RuleActionsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[カテゴリ](assigncategories.md)  |  を割り当てる[Copytofolder](copytofolder.md)  | [削除](delete.md)  | [Forwardasattachmenttorecipients 添付ファイル](forwardasattachmenttorecipients.md)  | [Forwardトーラス (pitor)](forwardtorecipients.md)  | [マーク (重要](markimportance.md)  |  )[Markasread](markasread.md)  | [Movetofolder](movetofolder.md)  | [PermanentDelete](permanentdelete.md)  | [Redirecttorて](redirecttorecipients.md)  |  いるイベント[SendSMSAlertToRecipients](sendsmsalerttorecipients.md)  | [ServerReplyWithMessage](serverreplywithmessage.md)  | [StopProcessingRules](stopprocessingrules.md)
  
### <a name="parent-elements"></a>親要素

[ルール (RuleType)](rule-ruletype.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

