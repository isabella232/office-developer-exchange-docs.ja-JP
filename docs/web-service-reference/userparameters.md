---
title: UserParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: UserParameters 要素には、有効と無効のクライアント拡張機能の一覧が含まれています。
ms.openlocfilehash: 76bf858adfb6d2ef76a25c234117131752c60d7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526754"
---
# <a name="userparameters"></a><span data-ttu-id="7f424-103">UserParameters</span><span class="sxs-lookup"><span data-stu-id="7f424-103">UserParameters</span></span>

<span data-ttu-id="7f424-104">**Userparameters**要素には、有効と無効のクライアント拡張機能の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7f424-104">The **UserParameters** element contains a list of enabled and disabled client extensions.</span></span> 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 <span data-ttu-id="7f424-105">**GetClientExtensionUserParametersType**</span><span class="sxs-lookup"><span data-stu-id="7f424-105">**GetClientExtensionUserParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f424-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7f424-106">Attributes and elements</span></span>

<span data-ttu-id="7f424-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7f424-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f424-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f424-108">Attributes</span></span>

|<span data-ttu-id="7f424-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="7f424-109">**Attribute**</span></span>|<span data-ttu-id="7f424-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="7f424-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7f424-111">UserId</span><span class="sxs-lookup"><span data-stu-id="7f424-111">UserId</span></span>  <br/> |<span data-ttu-id="7f424-112">**UserId**属性のテキスト値は、ユーザーの識別子です。</span><span class="sxs-lookup"><span data-stu-id="7f424-112">The text value of the **UserId** attribute is the identifier of the user.</span></span>  <br/> |
|<span data-ttu-id="7f424-113">EnabledOnly</span><span class="sxs-lookup"><span data-stu-id="7f424-113">EnabledOnly</span></span>  <br/> |<span data-ttu-id="7f424-114">**Enabledonly**テキスト値は、応答に有効な拡張機能のみが含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f424-114">The text value of the **EnabledOnly** indicates whether the response only contains the enabled extensions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7f424-115">子要素</span><span class="sxs-lookup"><span data-stu-id="7f424-115">Child elements</span></span>

<span data-ttu-id="7f424-116">[UserEnabledExtensions](userenabledextensions.md)  | [UserDisabledExtensions](userdisabledextensions.md)</span><span class="sxs-lookup"><span data-stu-id="7f424-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7f424-117">親要素</span><span class="sxs-lookup"><span data-stu-id="7f424-117">Parent elements</span></span>

[<span data-ttu-id="7f424-118">GetClientExtension</span><span class="sxs-lookup"><span data-stu-id="7f424-118">GetClientExtension</span></span>](getclientextension.md)
  
## <a name="remarks"></a><span data-ttu-id="7f424-119">注釈</span><span class="sxs-lookup"><span data-stu-id="7f424-119">Remarks</span></span>

<span data-ttu-id="7f424-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7f424-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7f424-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7f424-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f424-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7f424-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f424-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="7f424-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7f424-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7f424-124">Schema name</span></span>  <br/> |<span data-ttu-id="7f424-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7f424-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7f424-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7f424-126">Validation file</span></span>  <br/> |<span data-ttu-id="7f424-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7f424-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7f424-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7f424-128">Can be empty</span></span>  <br/> ||
   

