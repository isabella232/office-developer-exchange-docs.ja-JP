---
title: SetClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 10d0739c-2591-4768-935c-b131b26e974d
description: SetClientExtension 要素には、クライアント拡張機能を設定するための要求が含まれています。
ms.openlocfilehash: a856cd6b7063f7399e584b9932fcaf7fdc53094e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466165"
---
# <a name="setclientextension"></a><span data-ttu-id="94c60-103">SetClientExtension</span><span class="sxs-lookup"><span data-stu-id="94c60-103">SetClientExtension</span></span>

<span data-ttu-id="94c60-104">**Setclientextension**要素には、クライアント拡張機能を設定するための要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="94c60-104">The **SetClientExtension** element contains a request to set a client extension.</span></span> 
  
```XML
<SetClientExtension>
   <Actions/>
</SetClientExtension>
```

 <span data-ttu-id="94c60-105">**SetClientExtensionType**</span><span class="sxs-lookup"><span data-stu-id="94c60-105">**SetClientExtensionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94c60-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="94c60-106">Attributes and elements</span></span>

<span data-ttu-id="94c60-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="94c60-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94c60-108">属性</span><span class="sxs-lookup"><span data-stu-id="94c60-108">Attributes</span></span>

<span data-ttu-id="94c60-109">なし。</span><span class="sxs-lookup"><span data-stu-id="94c60-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94c60-110">子要素</span><span class="sxs-lookup"><span data-stu-id="94c60-110">Child elements</span></span>

[<span data-ttu-id="94c60-111">Actions (ArrayOfSetClientExtensionActionsType)</span><span class="sxs-lookup"><span data-stu-id="94c60-111">Actions (ArrayOfSetClientExtensionActionsType)</span></span>](actions-arrayofsetclientextensionactionstype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="94c60-112">親要素</span><span class="sxs-lookup"><span data-stu-id="94c60-112">Parent elements</span></span>

<span data-ttu-id="94c60-113">なし。</span><span class="sxs-lookup"><span data-stu-id="94c60-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="94c60-114">注釈</span><span class="sxs-lookup"><span data-stu-id="94c60-114">Remarks</span></span>

<span data-ttu-id="94c60-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="94c60-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="94c60-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="94c60-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94c60-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="94c60-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94c60-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="94c60-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="94c60-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="94c60-119">Schema name</span></span>  <br/> |<span data-ttu-id="94c60-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="94c60-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="94c60-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="94c60-121">Validation file</span></span>  <br/> |<span data-ttu-id="94c60-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="94c60-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="94c60-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="94c60-123">Can be empty</span></span>  <br/> |<span data-ttu-id="94c60-124">false</span><span class="sxs-lookup"><span data-stu-id="94c60-124">false</span></span>  <br/> |
   

