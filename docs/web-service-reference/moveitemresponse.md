---
title: MoveItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItemResponse
api_type:
- schema
ms.assetid: 77be5104-1e09-4d50-abec-4fadb3a230e5
description: MoveItemResponse 要素は、MoveItem 要求に対する応答を定義します。
ms.openlocfilehash: 1d7467fc1b0cb37392365c64c0e308a37171273b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466634"
---
# <a name="moveitemresponse"></a><span data-ttu-id="f573a-103">MoveItemResponse</span><span class="sxs-lookup"><span data-stu-id="f573a-103">MoveItemResponse</span></span>

<span data-ttu-id="f573a-104">**Moveitemresponse**要素は、moveitem 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="f573a-104">The **MoveItemResponse** element defines a response to a MoveItem request.</span></span> 
  
```xml
<MoveItemResponse>
   <ResponseMessages/>
</MoveItemResponse>
```

 <span data-ttu-id="f573a-105">**MoveItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="f573a-105">**MoveItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f573a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f573a-106">Attributes and elements</span></span>

<span data-ttu-id="f573a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f573a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f573a-108">属性</span><span class="sxs-lookup"><span data-stu-id="f573a-108">Attributes</span></span>

<span data-ttu-id="f573a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f573a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f573a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f573a-110">Child elements</span></span>

|<span data-ttu-id="f573a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f573a-111">**Element**</span></span>|<span data-ttu-id="f573a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f573a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f573a-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f573a-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f573a-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="f573a-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f573a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f573a-115">Parent elements</span></span>

<span data-ttu-id="f573a-116">なし。</span><span class="sxs-lookup"><span data-stu-id="f573a-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f573a-117">注釈</span><span class="sxs-lookup"><span data-stu-id="f573a-117">Remarks</span></span>

<span data-ttu-id="f573a-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f573a-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f573a-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f573a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f573a-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="f573a-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f573a-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f573a-121">Schema name</span></span>  <br/> |<span data-ttu-id="f573a-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f573a-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f573a-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f573a-123">Validation file</span></span>  <br/> |<span data-ttu-id="f573a-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f573a-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f573a-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f573a-125">Can be empty</span></span>  <br/> |<span data-ttu-id="f573a-126">いいえ</span><span class="sxs-lookup"><span data-stu-id="f573a-126">False</span></span>  <br/> |
   

