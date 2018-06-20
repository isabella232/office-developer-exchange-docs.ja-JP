---
title: 構成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: 構成要素は、ユーザーのメールボックスを識別します。
ms.openlocfilehash: 9f359a2b0ba315c236d4bf189c3de321417bd390
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839937"
---
# <a name="usermailbox"></a><span data-ttu-id="5b638-103">構成</span><span class="sxs-lookup"><span data-stu-id="5b638-103">UserMailbox</span></span>

<span data-ttu-id="5b638-104">**構成**要素は、ユーザーのメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="5b638-104">The **UserMailbox** element identifies a user mailbox.</span></span> 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 <span data-ttu-id="5b638-105">**UserMailboxType**</span><span class="sxs-lookup"><span data-stu-id="5b638-105">**UserMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b638-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5b638-106">Attributes and elements</span></span>

<span data-ttu-id="5b638-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5b638-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b638-108">属性</span><span class="sxs-lookup"><span data-stu-id="5b638-108">Attributes</span></span>

|<span data-ttu-id="5b638-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="5b638-109">**Attribute**</span></span>|<span data-ttu-id="5b638-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="5b638-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5b638-111">ID</span><span class="sxs-lookup"><span data-stu-id="5b638-111">Id</span></span>  <br/> |<span data-ttu-id="5b638-112">**Id**属性のテキスト値は、メールボックスの識別子です。</span><span class="sxs-lookup"><span data-stu-id="5b638-112">The text value of the **Id** attribute is the identifier of the mailbox.</span></span>  <br/> |
|<span data-ttu-id="5b638-113">IsArchive</span><span class="sxs-lookup"><span data-stu-id="5b638-113">IsArchive</span></span>  <br/> |<span data-ttu-id="5b638-114">**IsArchive**属性のテキスト値は、メールボックスは、アーカイブ メールボックスであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5b638-114">The text value of the **IsArchive** attribute indicates whether the mailbox is an archive mailbox.</span></span> <span data-ttu-id="5b638-115">テキストの値**は true** **IsArchive**属性には、メールボックスが、アーカイブ メールボックスであることを示します。</span><span class="sxs-lookup"><span data-stu-id="5b638-115">A text value of **true** for the **IsArchive** attribute indicates that the mailbox is an archive mailbox.</span></span> <span data-ttu-id="5b638-116">**False** **IsArchive** ] 属性の値は、メールボックスがプライマリ メールボックスであることを示します。</span><span class="sxs-lookup"><span data-stu-id="5b638-116">A value of **false** for the **IsArchive** attribute indicates that the mailbox is a primary mailbox.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5b638-117">子要素</span><span class="sxs-lookup"><span data-stu-id="5b638-117">Child elements</span></span>

<span data-ttu-id="5b638-118">なし。</span><span class="sxs-lookup"><span data-stu-id="5b638-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5b638-119">親要素</span><span class="sxs-lookup"><span data-stu-id="5b638-119">Parent elements</span></span>

<span data-ttu-id="5b638-120">[メールボックス (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span><span class="sxs-lookup"><span data-stu-id="5b638-120">[Mailboxes (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5b638-121">備考</span><span class="sxs-lookup"><span data-stu-id="5b638-121">Remarks</span></span>

<span data-ttu-id="5b638-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5b638-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5b638-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5b638-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b638-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="5b638-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b638-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="5b638-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5b638-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5b638-126">Schema name</span></span>  <br/> |<span data-ttu-id="5b638-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5b638-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="5b638-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5b638-128">Validation file</span></span>  <br/> |<span data-ttu-id="5b638-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5b638-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5b638-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5b638-130">Can be empty</span></span>  <br/> |<span data-ttu-id="5b638-131">true</span><span class="sxs-lookup"><span data-stu-id="5b638-131">true</span></span>  <br/> |
   

