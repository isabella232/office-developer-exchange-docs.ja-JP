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
# <a name="actions-ruleactionstype"></a><span data-ttu-id="b2b0b-103">Actions (RuleActionsType)</span><span class="sxs-lookup"><span data-stu-id="b2b0b-103">Actions (RuleActionsType)</span></span>

<span data-ttu-id="b2b0b-104">**Actions**要素には、受信トレイルールに関連付けられたアクションのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b2b0b-104">The **Actions** element contains a list of actions associated with Inbox rules.</span></span> 
  
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

 <span data-ttu-id="b2b0b-105">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="b2b0b-105">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b2b0b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b2b0b-106">Attributes and elements</span></span>

<span data-ttu-id="b2b0b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b2b0b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2b0b-108">属性</span><span class="sxs-lookup"><span data-stu-id="b2b0b-108">Attributes</span></span>

<span data-ttu-id="b2b0b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b2b0b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2b0b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b2b0b-110">Child elements</span></span>

<span data-ttu-id="b2b0b-111">[カテゴリ](assigncategories.md)  |  を割り当てる[Copytofolder](copytofolder.md)  | [削除](delete.md)  | [Forwardasattachmenttorecipients 添付ファイル](forwardasattachmenttorecipients.md)  | [Forwardトーラス (pitor)](forwardtorecipients.md)  | [マーク (重要](markimportance.md)  |  )[Markasread](markasread.md)  | [Movetofolder](movetofolder.md)  | [PermanentDelete](permanentdelete.md)  | [Redirecttorて](redirecttorecipients.md)  |  いるイベント[SendSMSAlertToRecipients](sendsmsalerttorecipients.md)  | [ServerReplyWithMessage](serverreplywithmessage.md)  | [StopProcessingRules](stopprocessingrules.md)</span><span class="sxs-lookup"><span data-stu-id="b2b0b-111">[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [Delete](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead](markasread.md) | [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md) | [StopProcessingRules](stopprocessingrules.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b2b0b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b2b0b-112">Parent elements</span></span>

[<span data-ttu-id="b2b0b-113">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="b2b0b-113">Rule (RuleType)</span></span>](rule-ruletype.md)
  
## <a name="remarks"></a><span data-ttu-id="b2b0b-114">注釈</span><span class="sxs-lookup"><span data-stu-id="b2b0b-114">Remarks</span></span>

<span data-ttu-id="b2b0b-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b2b0b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b2b0b-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b2b0b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2b0b-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b2b0b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2b0b-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="b2b0b-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b2b0b-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b2b0b-119">Schema name</span></span>  <br/> |<span data-ttu-id="b2b0b-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b2b0b-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="b2b0b-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b2b0b-121">Validation file</span></span>  <br/> |<span data-ttu-id="b2b0b-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b2b0b-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b2b0b-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b2b0b-123">Can be empty</span></span>  <br/> |<span data-ttu-id="b2b0b-124">false</span><span class="sxs-lookup"><span data-stu-id="b2b0b-124">false</span></span>  <br/> |
   

