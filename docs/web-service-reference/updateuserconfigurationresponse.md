---
title: UpdateUserConfigurationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateUserConfigurationResponse
api_type:
- schema
ms.assetid: 4a4b87d5-be95-4fde-a80b-e7f61dcd13e5
description: UpdateUserConfigurationResponse 要素は、1 つの UpdateUserConfiguration 要求への応答を定義します。
ms.openlocfilehash: 9a8a25443db05d8d7da28772b84edcf80cd9a921
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839894"
---
# <a name="updateuserconfigurationresponse"></a><span data-ttu-id="f0e29-103">UpdateUserConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="f0e29-103">UpdateUserConfigurationResponse</span></span>

<span data-ttu-id="f0e29-104">**UpdateUserConfigurationResponse**要素は、1 つの UpdateUserConfiguration 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="f0e29-104">The **UpdateUserConfigurationResponse** element defines a response to a single UpdateUserConfiguration request.</span></span> 
  
```xml
<UpdateUserConfigurationResponse>   <ResponseMessages/></UpdateUserConfigurationResponse>
```

 <span data-ttu-id="f0e29-105">**UpdateUserConfigurationResponseType**</span><span class="sxs-lookup"><span data-stu-id="f0e29-105">**UpdateUserConfigurationResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0e29-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f0e29-106">Attributes and elements</span></span>

<span data-ttu-id="f0e29-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f0e29-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0e29-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0e29-108">Attributes</span></span>

<span data-ttu-id="f0e29-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f0e29-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0e29-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f0e29-110">Child elements</span></span>

|<span data-ttu-id="f0e29-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f0e29-111">**Element**</span></span>|<span data-ttu-id="f0e29-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0e29-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0e29-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f0e29-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f0e29-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0e29-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0e29-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f0e29-115">Parent elements</span></span>

<span data-ttu-id="f0e29-116">なし。</span><span class="sxs-lookup"><span data-stu-id="f0e29-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f0e29-117">備考</span><span class="sxs-lookup"><span data-stu-id="f0e29-117">Remarks</span></span>

<span data-ttu-id="f0e29-118">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f0e29-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0e29-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="f0e29-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0e29-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="f0e29-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f0e29-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f0e29-121">Schema Name</span></span>  <br/> |<span data-ttu-id="f0e29-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f0e29-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f0e29-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f0e29-123">Validation File</span></span>  <br/> |<span data-ttu-id="f0e29-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f0e29-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f0e29-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f0e29-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0e29-126">False</span><span class="sxs-lookup"><span data-stu-id="f0e29-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0e29-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="f0e29-127">See also</span></span>



- [<span data-ttu-id="f0e29-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f0e29-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

