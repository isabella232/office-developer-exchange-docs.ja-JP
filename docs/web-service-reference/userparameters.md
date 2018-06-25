---
title: UserParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: UserParameters 要素には、有効および無効のクライアント拡張機能の一覧が含まれています。
ms.openlocfilehash: e0a72fe13255380ee56b32c863fb3bffb2e1ac5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839946"
---
# <a name="userparameters"></a><span data-ttu-id="e0fbc-103">UserParameters</span><span class="sxs-lookup"><span data-stu-id="e0fbc-103">UserParameters</span></span>

<span data-ttu-id="e0fbc-104">**UserParameters**要素には、有効および無効のクライアント拡張機能の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e0fbc-104">The **UserParameters** element contains a list of enabled and disabled client extensions.</span></span> 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 <span data-ttu-id="e0fbc-105">**GetClientExtensionUserParametersType**</span><span class="sxs-lookup"><span data-stu-id="e0fbc-105">**GetClientExtensionUserParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0fbc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e0fbc-106">Attributes and elements</span></span>

<span data-ttu-id="e0fbc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e0fbc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0fbc-108">属性</span><span class="sxs-lookup"><span data-stu-id="e0fbc-108">Attributes</span></span>

|<span data-ttu-id="e0fbc-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="e0fbc-109">**Attribute**</span></span>|<span data-ttu-id="e0fbc-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="e0fbc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e0fbc-111">UserId</span><span class="sxs-lookup"><span data-stu-id="e0fbc-111">UserId</span></span>  <br/> |<span data-ttu-id="e0fbc-112">**ユーザー Id**属性のテキスト値は、ユーザーの識別子です。</span><span class="sxs-lookup"><span data-stu-id="e0fbc-112">The text value of the **UserId** attribute is the identifier of the user.</span></span>  <br/> |
|<span data-ttu-id="e0fbc-113">EnabledOnly</span><span class="sxs-lookup"><span data-stu-id="e0fbc-113">EnabledOnly</span></span>  <br/> |<span data-ttu-id="e0fbc-114">**EnabledOnly**のテキスト値は、応答が有効になっている拡張機能のみを含むかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e0fbc-114">The text value of the **EnabledOnly** indicates whether the response only contains the enabled extensions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e0fbc-115">子要素</span><span class="sxs-lookup"><span data-stu-id="e0fbc-115">Child elements</span></span>

<span data-ttu-id="e0fbc-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span><span class="sxs-lookup"><span data-stu-id="e0fbc-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e0fbc-117">親要素</span><span class="sxs-lookup"><span data-stu-id="e0fbc-117">Parent elements</span></span>

[<span data-ttu-id="e0fbc-118">GetClientExtension</span><span class="sxs-lookup"><span data-stu-id="e0fbc-118">GetClientExtension</span></span>](getclientextension.md)
  
## <a name="remarks"></a><span data-ttu-id="e0fbc-119">備考</span><span class="sxs-lookup"><span data-stu-id="e0fbc-119">Remarks</span></span>

<span data-ttu-id="e0fbc-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e0fbc-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e0fbc-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e0fbc-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0fbc-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="e0fbc-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0fbc-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="e0fbc-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e0fbc-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e0fbc-124">Schema name</span></span>  <br/> |<span data-ttu-id="e0fbc-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e0fbc-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="e0fbc-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e0fbc-126">Validation file</span></span>  <br/> |<span data-ttu-id="e0fbc-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e0fbc-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e0fbc-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e0fbc-128">Can be empty</span></span>  <br/> ||
   

