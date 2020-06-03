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
description: Mailbox 要素には、検出対象のユーザーの電子メールアドレスが含まれています。
ms.openlocfilehash: e050cd9d3ca4a2d2450f315f1eedd3862328d096
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467285"
---
# <a name="mailbox-soap"></a><span data-ttu-id="e691b-103">メールボックス (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e691b-103">Mailbox (SOAP)</span></span>

<span data-ttu-id="e691b-104">**Mailbox**要素には、検出対象のユーザーの電子メールアドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e691b-104">The **Mailbox** element contains the e-mail address of the user to be discovered.</span></span> 
  
```XML
<Mailbox/>
```

<span data-ttu-id="e691b-105">**string**</span><span class="sxs-lookup"><span data-stu-id="e691b-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e691b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e691b-106">Attributes and elements</span></span>

<span data-ttu-id="e691b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e691b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e691b-108">属性</span><span class="sxs-lookup"><span data-stu-id="e691b-108">Attributes</span></span>

<span data-ttu-id="e691b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e691b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e691b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e691b-110">Child elements</span></span>

<span data-ttu-id="e691b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e691b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e691b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e691b-112">Parent elements</span></span>

|<span data-ttu-id="e691b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e691b-113">**Element**</span></span>|<span data-ttu-id="e691b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e691b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e691b-115">User (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e691b-115">User (SOAP)</span></span>](user-soap.md) <br/> |<span data-ttu-id="e691b-116">1人のユーザーの id を表します。</span><span class="sxs-lookup"><span data-stu-id="e691b-116">Represents the identity of a single user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e691b-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e691b-117">Text value</span></span>

<span data-ttu-id="e691b-118">**Mailbox**要素のテキスト値は、検出されるユーザーの電子メールアドレスです。</span><span class="sxs-lookup"><span data-stu-id="e691b-118">The text value of the **Mailbox** element is the e-mail address of the user to be discovered.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e691b-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e691b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e691b-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="e691b-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e691b-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e691b-121">Schema Name</span></span>  <br/> |<span data-ttu-id="e691b-122">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="e691b-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e691b-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e691b-123">Validation File</span></span>  <br/> |<span data-ttu-id="e691b-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="e691b-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e691b-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e691b-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="e691b-126">正しい</span><span class="sxs-lookup"><span data-stu-id="e691b-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e691b-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="e691b-127">See also</span></span>

- [<span data-ttu-id="e691b-128">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e691b-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

