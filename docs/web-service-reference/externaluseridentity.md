---
title: ExternalUserIdentity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExternalUserIdentity
api_type:
- schema
ms.assetid: f2bc0a61-7c50-4b36-828e-358dfc5b9ae1
description: ExternalUserIdentity 要素は、外部の代理人のユーザー、またはフォルダーのアクセス許可を持つ外部ユーザーを識別します。
ms.openlocfilehash: 08ca4500ba610150e9e673f1b63823dabf70d9ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760456"
---
# <a name="externaluseridentity"></a><span data-ttu-id="c20ac-103">ExternalUserIdentity</span><span class="sxs-lookup"><span data-stu-id="c20ac-103">ExternalUserIdentity</span></span>

<span data-ttu-id="c20ac-104">**ExternalUserIdentity**要素は、外部の代理人のユーザー、またはフォルダーのアクセス許可を持つ外部ユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c20ac-104">The **ExternalUserIdentity** element identifies an external delegate user or an external user who has folder access permissions.</span></span> 
  
```xml
<ExternalUserIdentity/>
```

 <span data-ttu-id="c20ac-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="c20ac-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c20ac-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c20ac-106">Attributes and elements</span></span>

<span data-ttu-id="c20ac-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c20ac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c20ac-108">属性</span><span class="sxs-lookup"><span data-stu-id="c20ac-108">Attributes</span></span>

<span data-ttu-id="c20ac-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c20ac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c20ac-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c20ac-110">Child elements</span></span>

<span data-ttu-id="c20ac-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c20ac-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c20ac-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c20ac-112">Parent elements</span></span>

|<span data-ttu-id="c20ac-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c20ac-113">**Element**</span></span>|<span data-ttu-id="c20ac-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c20ac-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c20ac-115">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="c20ac-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="c20ac-116">代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c20ac-116">Identifies a delegate user or a user who has folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c20ac-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c20ac-117">Text value</span></span>

<span data-ttu-id="c20ac-118">なし。</span><span class="sxs-lookup"><span data-stu-id="c20ac-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c20ac-119">備考</span><span class="sxs-lookup"><span data-stu-id="c20ac-119">Remarks</span></span>

<span data-ttu-id="c20ac-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c20ac-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c20ac-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="c20ac-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c20ac-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="c20ac-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c20ac-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c20ac-123">Schema Name</span></span>  <br/> |<span data-ttu-id="c20ac-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c20ac-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="c20ac-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c20ac-125">Validation File</span></span>  <br/> |<span data-ttu-id="c20ac-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c20ac-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c20ac-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c20ac-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="c20ac-128">False</span><span class="sxs-lookup"><span data-stu-id="c20ac-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c20ac-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="c20ac-129">See also</span></span>



- [<span data-ttu-id="c20ac-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c20ac-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

