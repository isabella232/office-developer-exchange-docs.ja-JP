---
title: 電子メール (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c40a6b6-e2d1-44ba-b439-5720490cbd43
description: Email 要素は、会議の出席者を識別します。
ms.openlocfilehash: 9457ff735f4f87f59cd091b504fb8807e1aa8fa6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459238"
---
# <a name="email-emailaddress"></a><span data-ttu-id="822c7-103">電子メール (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="822c7-103">Email (EmailAddress)</span></span>

<span data-ttu-id="822c7-104">**Email**要素は、会議の出席者を識別します。</span><span class="sxs-lookup"><span data-stu-id="822c7-104">The **Email** element identifies an attendee to a meeting.</span></span> 
  
```XML
<Email></Email>
```

 <span data-ttu-id="822c7-105">**EmailAddress**</span><span class="sxs-lookup"><span data-stu-id="822c7-105">**EmailAddress**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="822c7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="822c7-106">Attributes and elements</span></span>

<span data-ttu-id="822c7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="822c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="822c7-108">属性</span><span class="sxs-lookup"><span data-stu-id="822c7-108">Attributes</span></span>

<span data-ttu-id="822c7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="822c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="822c7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="822c7-110">Child elements</span></span>

<span data-ttu-id="822c7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="822c7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="822c7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="822c7-112">Parent elements</span></span>

[<span data-ttu-id="822c7-113">MailboxData</span><span class="sxs-lookup"><span data-stu-id="822c7-113">MailboxData</span></span>](mailboxdata.md)
  
## <a name="text-value"></a><span data-ttu-id="822c7-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="822c7-114">Text value</span></span>

<span data-ttu-id="822c7-115">Email 要素のテキスト値は、 **Getuseravailability**操作応答で返される出席者を識別します。</span><span class="sxs-lookup"><span data-stu-id="822c7-115">The text value of the Email element identifies an attendee returned in a **GetUserAvailability** operation response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="822c7-116">注釈</span><span class="sxs-lookup"><span data-stu-id="822c7-116">Remarks</span></span>

<span data-ttu-id="822c7-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="822c7-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="822c7-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="822c7-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="822c7-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="822c7-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="822c7-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="822c7-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="822c7-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="822c7-121">Schema name</span></span>  <br/> |<span data-ttu-id="822c7-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="822c7-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="822c7-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="822c7-123">Validation file</span></span>  <br/> |<span data-ttu-id="822c7-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="822c7-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="822c7-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="822c7-125">Can be empty</span></span>  <br/> ||
   

