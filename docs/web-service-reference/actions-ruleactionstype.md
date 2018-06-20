---
title: アクション (RuleActionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2afba70c-65f7-458c-a4e6-a2cd9bccc0f9
description: アクション要素には、受信トレイのルールに関連付けられているアクションの一覧が含まれています。
ms.openlocfilehash: 8ed8095ca8b41e037c2c0dad319c9c4ab99ed2bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759361"
---
# <a name="actions-ruleactionstype"></a><span data-ttu-id="6f93e-103">アクション (RuleActionsType)</span><span class="sxs-lookup"><span data-stu-id="6f93e-103">Actions (RuleActionsType)</span></span>

<span data-ttu-id="6f93e-104">**アクション**要素には、受信トレイのルールに関連付けられているアクションの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6f93e-104">The **Actions** element contains a list of actions associated with Inbox rules.</span></span> 
  
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

 <span data-ttu-id="6f93e-105">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="6f93e-105">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f93e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6f93e-106">Attributes and elements</span></span>

<span data-ttu-id="6f93e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6f93e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f93e-108">属性</span><span class="sxs-lookup"><span data-stu-id="6f93e-108">Attributes</span></span>

<span data-ttu-id="6f93e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6f93e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f93e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6f93e-110">Child elements</span></span>

<span data-ttu-id="6f93e-111">[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [削除](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead](markasread.md)  |  [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md)  |  [StopProcessingRules](stopprocessingrules.md)</span><span class="sxs-lookup"><span data-stu-id="6f93e-111">[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [Delete](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead](markasread.md) | [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md) | [StopProcessingRules](stopprocessingrules.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6f93e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6f93e-112">Parent elements</span></span>

[<span data-ttu-id="6f93e-113">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="6f93e-113">Rule (RuleType)</span></span>](rule-ruletype.md)
  
## <a name="remarks"></a><span data-ttu-id="6f93e-114">備考</span><span class="sxs-lookup"><span data-stu-id="6f93e-114">Remarks</span></span>

<span data-ttu-id="6f93e-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6f93e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6f93e-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6f93e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f93e-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="6f93e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f93e-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="6f93e-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f93e-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6f93e-119">Schema name</span></span>  <br/> |<span data-ttu-id="6f93e-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6f93e-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f93e-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6f93e-121">Validation file</span></span>  <br/> |<span data-ttu-id="6f93e-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6f93e-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f93e-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6f93e-123">Can be empty</span></span>  <br/> |<span data-ttu-id="6f93e-124">false</span><span class="sxs-lookup"><span data-stu-id="6f93e-124">false</span></span>  <br/> |
   

