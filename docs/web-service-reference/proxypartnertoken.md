---
title: ProxyPartnerToken
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 88d35c05-21fc-4576-b785-c4ba7b6f8d5b
description: ProxyPartnerToken 要素は、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの HTTP プロキシによって使用されます。 Exchange Web サービス (EWS) の操作では、この要素は使用されません。
ms.openlocfilehash: d21f7ab57b9abd5521a9e7551f317be41a937e12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832916"
---
# <a name="proxypartnertoken"></a><span data-ttu-id="c7725-104">ProxyPartnerToken</span><span class="sxs-lookup"><span data-stu-id="c7725-104">ProxyPartnerToken</span></span>

<span data-ttu-id="c7725-105">**ProxyPartnerToken**要素は、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの HTTP プロキシによって使用されます。</span><span class="sxs-lookup"><span data-stu-id="c7725-105">The **ProxyPartnerToken** element is used by HTTP proxy of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> <span data-ttu-id="c7725-106">Exchange Web サービス (EWS) の操作では、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="c7725-106">This element is not used by Exchange Web Services (EWS) operations.</span></span> 
  
```XML
<ProxyPartnerToken/>
```

 <span data-ttu-id="c7725-107">**ProxySecurityContextType**</span><span class="sxs-lookup"><span data-stu-id="c7725-107">**ProxySecurityContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7725-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c7725-108">Attributes and elements</span></span>

<span data-ttu-id="c7725-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c7725-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7725-110">属性</span><span class="sxs-lookup"><span data-stu-id="c7725-110">Attributes</span></span>

<span data-ttu-id="c7725-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c7725-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7725-112">子要素</span><span class="sxs-lookup"><span data-stu-id="c7725-112">Child elements</span></span>

<span data-ttu-id="c7725-113">なし。</span><span class="sxs-lookup"><span data-stu-id="c7725-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c7725-114">親要素</span><span class="sxs-lookup"><span data-stu-id="c7725-114">Parent elements</span></span>

<span data-ttu-id="c7725-115">なし。</span><span class="sxs-lookup"><span data-stu-id="c7725-115">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c7725-116">備考</span><span class="sxs-lookup"><span data-stu-id="c7725-116">Remarks</span></span>

<span data-ttu-id="c7725-117">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c7725-117">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="c7725-118">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c7725-118">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7725-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="c7725-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7725-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="c7725-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c7725-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c7725-121">Schema Name</span></span>  <br/> |<span data-ttu-id="c7725-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c7725-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="c7725-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c7725-123">Validation File</span></span>  <br/> |<span data-ttu-id="c7725-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c7725-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c7725-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c7725-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="c7725-126">False</span><span class="sxs-lookup"><span data-stu-id="c7725-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7725-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="c7725-127">See also</span></span>



- [<span data-ttu-id="c7725-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c7725-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

