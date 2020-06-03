---
title: AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: adbffbfc-e436-4620-acfc-5dfd41a88cb8
description: Adddistribution Grouptoimlist 要素は、インスタントメッセージリストに配布リストを追加する要求を定義します。
ms.openlocfilehash: 90a84b23678fb0740158f601967905a8847286fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460380"
---
# <a name="adddistributiongrouptoimlist"></a><span data-ttu-id="161a6-103">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="161a6-103">AddDistributionGroupToImList</span></span>

<span data-ttu-id="161a6-104">**Adddistribution Grouptoimlist**要素は、インスタントメッセージリストに配布リストを追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="161a6-104">The **AddDistributionGroupToImList** element defines a request to add a distribution list to an instant message list.</span></span> 
  
```XML
<AddDistributionGroupToImList>
   <SmtpAddress/>
   <DisplayName/>
</AddDistributionGroupToImList>
```

 <span data-ttu-id="161a6-105">**Adddeploy Grouptoimlisttype**</span><span class="sxs-lookup"><span data-stu-id="161a6-105">**AddDistributionGroupToImListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="161a6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="161a6-106">Attributes and elements</span></span>

<span data-ttu-id="161a6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="161a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="161a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="161a6-108">Attributes</span></span>

<span data-ttu-id="161a6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="161a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="161a6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="161a6-110">Child elements</span></span>

<span data-ttu-id="161a6-111">[Smtpaddress](smtpaddress.md)  | [DisplayName (非 Emptystringtype)](displayname-nonemptystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="161a6-111">[SmtpAddress](smtpaddress.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="161a6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="161a6-112">Parent elements</span></span>

<span data-ttu-id="161a6-113">なし。</span><span class="sxs-lookup"><span data-stu-id="161a6-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="161a6-114">注釈</span><span class="sxs-lookup"><span data-stu-id="161a6-114">Remarks</span></span>

<span data-ttu-id="161a6-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="161a6-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="161a6-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="161a6-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="161a6-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="161a6-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="161a6-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="161a6-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="161a6-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="161a6-119">Schema name</span></span>  <br/> |<span data-ttu-id="161a6-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="161a6-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="161a6-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="161a6-121">Validation file</span></span>  <br/> |<span data-ttu-id="161a6-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="161a6-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="161a6-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="161a6-123">Can be empty</span></span>  <br/> |<span data-ttu-id="161a6-124">false</span><span class="sxs-lookup"><span data-stu-id="161a6-124">false</span></span>  <br/> |
   

