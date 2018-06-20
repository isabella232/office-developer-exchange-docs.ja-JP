---
title: GetUserConfigurationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfigurationResponse
api_type:
- schema
ms.assetid: 5e418c91-c836-4de0-a80d-f0dad0c684d7
description: GetUserConfigurationResponse 要素は、1 つの GetUserConfiguration 要求への応答を定義します。
ms.openlocfilehash: b720809a66c75dbf75f6e597a0064992b9f741e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831689"
---
# <a name="getuserconfigurationresponse"></a><span data-ttu-id="0003d-103">GetUserConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="0003d-103">GetUserConfigurationResponse</span></span>

<span data-ttu-id="0003d-104">**GetUserConfigurationResponse**要素は、1 つの GetUserConfiguration 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="0003d-104">The **GetUserConfigurationResponse** element defines a response to a single GetUserConfiguration request.</span></span> 
  
```xml
<GetUserConfigurationResponse>   <ResponseMessages/></GetUserConfigurationResponse>
```

 <span data-ttu-id="0003d-105">**GetUserConfigurationResponseType**</span><span class="sxs-lookup"><span data-stu-id="0003d-105">**GetUserConfigurationResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0003d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0003d-106">Attributes and elements</span></span>

<span data-ttu-id="0003d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0003d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0003d-108">属性</span><span class="sxs-lookup"><span data-stu-id="0003d-108">Attributes</span></span>

<span data-ttu-id="0003d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0003d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0003d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0003d-110">Child elements</span></span>

|<span data-ttu-id="0003d-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="0003d-111">**Element**</span></span>|<span data-ttu-id="0003d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0003d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0003d-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0003d-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0003d-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0003d-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0003d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="0003d-115">Parent elements</span></span>

<span data-ttu-id="0003d-116">なし。</span><span class="sxs-lookup"><span data-stu-id="0003d-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0003d-117">備考</span><span class="sxs-lookup"><span data-stu-id="0003d-117">Remarks</span></span>

<span data-ttu-id="0003d-118">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0003d-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0003d-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="0003d-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0003d-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="0003d-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0003d-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0003d-121">Schema Name</span></span>  <br/> |<span data-ttu-id="0003d-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="0003d-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0003d-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0003d-123">Validation File</span></span>  <br/> |<span data-ttu-id="0003d-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0003d-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0003d-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0003d-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="0003d-126">False</span><span class="sxs-lookup"><span data-stu-id="0003d-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0003d-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="0003d-127">See also</span></span>



- [<span data-ttu-id="0003d-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0003d-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

