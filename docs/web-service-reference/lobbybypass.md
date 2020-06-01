---
title: LobbyBypass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: LobbyBypass 要素は、仮想ロビーをバイパスするオンライン会議の設定を指定します。
ms.openlocfilehash: 6940428c944b9d4d64acc6dbbf3993576e1932eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458097"
---
# <a name="lobbybypass"></a><span data-ttu-id="f2fda-103">LobbyBypass</span><span class="sxs-lookup"><span data-stu-id="f2fda-103">LobbyBypass</span></span>

<span data-ttu-id="f2fda-104">**Lobbybypass**要素は、仮想ロビーをバイパスするオンライン会議の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="f2fda-104">The **LobbyBypass** element specifies the online meeting setting to bypass the virtual lobby.</span></span> 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 <span data-ttu-id="f2fda-105">**LobbyBypassType**</span><span class="sxs-lookup"><span data-stu-id="f2fda-105">**LobbyBypassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2fda-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f2fda-106">Attributes and elements</span></span>

<span data-ttu-id="f2fda-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f2fda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2fda-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2fda-108">Attributes</span></span>

<span data-ttu-id="f2fda-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f2fda-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2fda-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f2fda-110">Child elements</span></span>

<span data-ttu-id="f2fda-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f2fda-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f2fda-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f2fda-112">Parent elements</span></span>

[<span data-ttu-id="f2fda-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="f2fda-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="f2fda-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f2fda-114">Text value</span></span>

<span data-ttu-id="f2fda-115">**Lobbybypass**要素のテキスト値は、Disabled または**EnabledForGatewayParticipants**のいずれか**に**なります。</span><span class="sxs-lookup"><span data-stu-id="f2fda-115">The text value of the **LobbyBypass** element can be either **Disabled** or **EnabledForGatewayParticipants**.</span></span> <span data-ttu-id="f2fda-116">**Disabled**値は、すべての会議の出席者が仮想ロビーを介してアクセスする必要があるように、ロビーバイパスが無効になっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="f2fda-116">The **Disabled** value indicates that the lobby bypass is disabled so all meeting attendees must access through the virtual lobby.</span></span> <span data-ttu-id="f2fda-117">**EnabledForGatewayParticipants**の値は、電話の参加者に対してロビーバイパスが有効になっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="f2fda-117">The **EnabledForGatewayParticipants** value indicates that the lobby bypass is enabled for telephone participants.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f2fda-118">注釈</span><span class="sxs-lookup"><span data-stu-id="f2fda-118">Remarks</span></span>

<span data-ttu-id="f2fda-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f2fda-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f2fda-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f2fda-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

