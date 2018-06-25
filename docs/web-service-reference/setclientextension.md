---
title: SetClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 10d0739c-2591-4768-935c-b131b26e974d
description: SetClientExtension 要素には、クライアントの拡張機能を設定するための要求が含まれています。
ms.openlocfilehash: 9e0a2926e25d74657ddf8a50ec88e77af0fc4ea1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833398"
---
# <a name="setclientextension"></a><span data-ttu-id="075a8-103">SetClientExtension</span><span class="sxs-lookup"><span data-stu-id="075a8-103">SetClientExtension</span></span>

<span data-ttu-id="075a8-104">**SetClientExtension**要素には、クライアントの拡張機能を設定するための要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="075a8-104">The **SetClientExtension** element contains a request to set a client extension.</span></span> 
  
```XML
<SetClientExtension>
   <Actions/>
</SetClientExtension>
```

 <span data-ttu-id="075a8-105">**SetClientExtensionType**</span><span class="sxs-lookup"><span data-stu-id="075a8-105">**SetClientExtensionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="075a8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="075a8-106">Attributes and elements</span></span>

<span data-ttu-id="075a8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="075a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="075a8-108">属性</span><span class="sxs-lookup"><span data-stu-id="075a8-108">Attributes</span></span>

<span data-ttu-id="075a8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="075a8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="075a8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="075a8-110">Child elements</span></span>

[<span data-ttu-id="075a8-111">アクション (ArrayOfSetClientExtensionActionsType)</span><span class="sxs-lookup"><span data-stu-id="075a8-111">Actions (ArrayOfSetClientExtensionActionsType)</span></span>](actions-arrayofsetclientextensionactionstype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="075a8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="075a8-112">Parent elements</span></span>

<span data-ttu-id="075a8-113">なし。</span><span class="sxs-lookup"><span data-stu-id="075a8-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="075a8-114">備考</span><span class="sxs-lookup"><span data-stu-id="075a8-114">Remarks</span></span>

<span data-ttu-id="075a8-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="075a8-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="075a8-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="075a8-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="075a8-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="075a8-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="075a8-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="075a8-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="075a8-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="075a8-119">Schema name</span></span>  <br/> |<span data-ttu-id="075a8-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="075a8-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="075a8-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="075a8-121">Validation file</span></span>  <br/> |<span data-ttu-id="075a8-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="075a8-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="075a8-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="075a8-123">Can be empty</span></span>  <br/> |<span data-ttu-id="075a8-124">false</span><span class="sxs-lookup"><span data-stu-id="075a8-124">false</span></span>  <br/> |
   

