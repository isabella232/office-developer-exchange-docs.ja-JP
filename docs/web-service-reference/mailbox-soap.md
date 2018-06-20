---
title: メールボックス (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4ad59e5b-4047-4c34-a318-ca06c31d3de8
description: メールボックスの要素には、検出対象のユーザーの電子メール アドレスが含まれています。
ms.openlocfilehash: b98397dadf8c467031eb8febe9732d4e426372e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832253"
---
# <a name="mailbox-soap"></a><span data-ttu-id="67ec6-103">メールボックス (SOAP)</span><span class="sxs-lookup"><span data-stu-id="67ec6-103">Mailbox (SOAP)</span></span>

<span data-ttu-id="67ec6-104">**メールボックス**の要素には、検出対象のユーザーの電子メール アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="67ec6-104">The **Mailbox** element contains the e-mail address of the user to be discovered.</span></span> 
  
```XML
<Mailbox/>
```

<span data-ttu-id="67ec6-105">**string**</span><span class="sxs-lookup"><span data-stu-id="67ec6-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="67ec6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="67ec6-106">Attributes and elements</span></span>

<span data-ttu-id="67ec6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="67ec6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67ec6-108">属性</span><span class="sxs-lookup"><span data-stu-id="67ec6-108">Attributes</span></span>

<span data-ttu-id="67ec6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="67ec6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67ec6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="67ec6-110">Child elements</span></span>

<span data-ttu-id="67ec6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="67ec6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="67ec6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="67ec6-112">Parent elements</span></span>

|<span data-ttu-id="67ec6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="67ec6-113">**Element**</span></span>|<span data-ttu-id="67ec6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="67ec6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67ec6-115">ユーザー (SOAP)</span><span class="sxs-lookup"><span data-stu-id="67ec6-115">User (SOAP)</span></span>](user-soap.md) <br/> |<span data-ttu-id="67ec6-116">1 人のユーザーの id を表します。</span><span class="sxs-lookup"><span data-stu-id="67ec6-116">Represents the identity of a single user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="67ec6-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="67ec6-117">Text value</span></span>

<span data-ttu-id="67ec6-118">**メールボックス**要素のテキスト値は、検出対象のユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="67ec6-118">The text value of the **Mailbox** element is the e-mail address of the user to be discovered.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="67ec6-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="67ec6-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67ec6-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="67ec6-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="67ec6-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="67ec6-121">Schema Name</span></span>  <br/> |<span data-ttu-id="67ec6-122">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="67ec6-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="67ec6-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="67ec6-123">Validation File</span></span>  <br/> |<span data-ttu-id="67ec6-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="67ec6-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="67ec6-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="67ec6-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="67ec6-126">True</span><span class="sxs-lookup"><span data-stu-id="67ec6-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67ec6-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="67ec6-127">See also</span></span>

- [<span data-ttu-id="67ec6-128">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="67ec6-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

