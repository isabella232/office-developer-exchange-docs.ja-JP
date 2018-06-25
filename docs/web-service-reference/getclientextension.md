---
title: GetClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c96c2b4c-45cb-482a-a3bb-7a11a0fff43b
description: GetClientExtension 要素は、クライアントの拡張機能を取得する要求を表します。
ms.openlocfilehash: 9d3abb4572a5f74f24925d24a2fbbe8ded593731
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760662"
---
# <a name="getclientextension"></a><span data-ttu-id="5cfbd-103">GetClientExtension</span><span class="sxs-lookup"><span data-stu-id="5cfbd-103">GetClientExtension</span></span>

<span data-ttu-id="5cfbd-104">**GetClientExtension**要素は、クライアントの拡張機能を取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="5cfbd-104">The **GetClientExtension** element represents a request to get a client extension.</span></span> 
  
```XML
<GetClientExtension>
   <RequestedExtensionIds/>
   <UserParameters/>
   <IsDebug/>
</GetClientExtension>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="5cfbd-105">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5cfbd-105">Attributes and elements</span></span>

<span data-ttu-id="5cfbd-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5cfbd-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cfbd-107">属性</span><span class="sxs-lookup"><span data-stu-id="5cfbd-107">Attributes</span></span>

<span data-ttu-id="5cfbd-108">なし。</span><span class="sxs-lookup"><span data-stu-id="5cfbd-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5cfbd-109">子要素</span><span class="sxs-lookup"><span data-stu-id="5cfbd-109">Child elements</span></span>

<span data-ttu-id="5cfbd-110">[RequestedExtensionIds](requestedextensionids.md) | [UserParameters](userparameters.md) | [IsDebug](isdebug.md)</span><span class="sxs-lookup"><span data-stu-id="5cfbd-110">[RequestedExtensionIds](requestedextensionids.md) | [UserParameters](userparameters.md) | [IsDebug](isdebug.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5cfbd-111">親要素</span><span class="sxs-lookup"><span data-stu-id="5cfbd-111">Parent elements</span></span>

<span data-ttu-id="5cfbd-112">なし。</span><span class="sxs-lookup"><span data-stu-id="5cfbd-112">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5cfbd-113">備考</span><span class="sxs-lookup"><span data-stu-id="5cfbd-113">Remarks</span></span>

<span data-ttu-id="5cfbd-114">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5cfbd-114">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5cfbd-115">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5cfbd-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cfbd-116">要素情報</span><span class="sxs-lookup"><span data-stu-id="5cfbd-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cfbd-117">名前空間</span><span class="sxs-lookup"><span data-stu-id="5cfbd-117">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5cfbd-118">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5cfbd-118">Schema name</span></span>  <br/> |<span data-ttu-id="5cfbd-119">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="5cfbd-119">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5cfbd-120">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5cfbd-120">Validation file</span></span>  <br/> |<span data-ttu-id="5cfbd-121">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5cfbd-121">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5cfbd-122">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5cfbd-122">Can be empty</span></span>  <br/> ||
   

