---
title: LobbyBypass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: LobbyBypass 要素は、オンライン会議、仮想ロビーをバイパスする設定を指定します。
ms.openlocfilehash: 9ecc920acd9e1aea3476ad1194d6c7d0529b21c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832246"
---
# <a name="lobbybypass"></a><span data-ttu-id="b8823-103">LobbyBypass</span><span class="sxs-lookup"><span data-stu-id="b8823-103">LobbyBypass</span></span>

<span data-ttu-id="b8823-104">**LobbyBypass**要素は、オンライン会議、仮想ロビーをバイパスする設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="b8823-104">The **LobbyBypass** element specifies the online meeting setting to bypass the virtual lobby.</span></span> 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 <span data-ttu-id="b8823-105">**LobbyBypassType**</span><span class="sxs-lookup"><span data-stu-id="b8823-105">**LobbyBypassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8823-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b8823-106">Attributes and elements</span></span>

<span data-ttu-id="b8823-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b8823-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8823-108">属性</span><span class="sxs-lookup"><span data-stu-id="b8823-108">Attributes</span></span>

<span data-ttu-id="b8823-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b8823-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8823-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b8823-110">Child elements</span></span>

<span data-ttu-id="b8823-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b8823-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b8823-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b8823-112">Parent elements</span></span>

[<span data-ttu-id="b8823-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="b8823-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="b8823-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b8823-114">Text value</span></span>

<span data-ttu-id="b8823-115">**LobbyBypass**要素のテキスト値には、**無効**または**EnabledForGatewayParticipants**のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="b8823-115">The text value of the **LobbyBypass** element can be either **Disabled** or **EnabledForGatewayParticipants**.</span></span> <span data-ttu-id="b8823-116">**無効になっている**値は、仮想ロビーをすべての会議出席者がアクセスする必要がありますので、ロビーのバイパスが無効になっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="b8823-116">The **Disabled** value indicates that the lobby bypass is disabled so all meeting attendees must access through the virtual lobby.</span></span> <span data-ttu-id="b8823-117">**EnabledForGatewayParticipants**値では、参加者の電話でロビーのバイパスが有効であることを示します。</span><span class="sxs-lookup"><span data-stu-id="b8823-117">The **EnabledForGatewayParticipants** value indicates that the lobby bypass is enabled for telephone participants.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b8823-118">備考</span><span class="sxs-lookup"><span data-stu-id="b8823-118">Remarks</span></span>

<span data-ttu-id="b8823-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b8823-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b8823-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b8823-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

