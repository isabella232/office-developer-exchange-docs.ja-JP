---
title: AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: adbffbfc-e436-4620-acfc-5dfd41a88cb8
description: AddDistributionGroupToImList 要素は、配布リストを [インスタント メッセージ] ボックスの一覧に追加する要求を定義します。
ms.openlocfilehash: b63daeb8b1d60123215bfcdec307f2f948d2ec39
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759280"
---
# <a name="adddistributiongrouptoimlist"></a><span data-ttu-id="8ea04-103">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="8ea04-103">AddDistributionGroupToImList</span></span>

<span data-ttu-id="8ea04-104">**AddDistributionGroupToImList**要素は、配布リストを [インスタント メッセージ] ボックスの一覧に追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="8ea04-104">The **AddDistributionGroupToImList** element defines a request to add a distribution list to an instant message list.</span></span> 
  
```XML
<AddDistributionGroupToImList>
   <SmtpAddress/>
   <DisplayName/>
</AddDistributionGroupToImList>
```

 <span data-ttu-id="8ea04-105">**AddDistributionGroupToImListType**</span><span class="sxs-lookup"><span data-stu-id="8ea04-105">**AddDistributionGroupToImListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ea04-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8ea04-106">Attributes and elements</span></span>

<span data-ttu-id="8ea04-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8ea04-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ea04-108">属性</span><span class="sxs-lookup"><span data-stu-id="8ea04-108">Attributes</span></span>

<span data-ttu-id="8ea04-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8ea04-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ea04-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8ea04-110">Child elements</span></span>

<span data-ttu-id="8ea04-111">[SmtpAddress](smtpaddress.md) | [(NonEmptyStringType) の表示名](displayname-nonemptystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="8ea04-111">[SmtpAddress](smtpaddress.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ea04-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8ea04-112">Parent elements</span></span>

<span data-ttu-id="8ea04-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8ea04-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8ea04-114">備考</span><span class="sxs-lookup"><span data-stu-id="8ea04-114">Remarks</span></span>

<span data-ttu-id="8ea04-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8ea04-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8ea04-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8ea04-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ea04-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="8ea04-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ea04-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="8ea04-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8ea04-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8ea04-119">Schema name</span></span>  <br/> |<span data-ttu-id="8ea04-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="8ea04-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8ea04-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8ea04-121">Validation file</span></span>  <br/> |<span data-ttu-id="8ea04-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8ea04-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8ea04-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8ea04-123">Can be empty</span></span>  <br/> |<span data-ttu-id="8ea04-124">false</span><span class="sxs-lookup"><span data-stu-id="8ea04-124">false</span></span>  <br/> |
   

