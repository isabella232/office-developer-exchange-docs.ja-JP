---
title: MoveFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolderResponse
api_type:
- schema
ms.assetid: e7dd2fb8-e362-42e5-a480-4d816813526d
description: MoveFolderResponse 要素は、MoveFolder 要求への応答を定義します。
ms.openlocfilehash: 2019321dcb03ec5e63b47a6b7579c8bd46756391
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461738"
---
# <a name="movefolderresponse"></a><span data-ttu-id="a0d5b-103">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="a0d5b-103">MoveFolderResponse</span></span>

<span data-ttu-id="a0d5b-104">**Movefolderresponse**要素は、movefolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="a0d5b-104">The **MoveFolderResponse** element defines a response to a MoveFolder request.</span></span> 
  
```xml
<MoveFolderResponse>
   <ResponseMessages/>
</MoveFolderResponse>
```

 <span data-ttu-id="a0d5b-105">**MoveFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="a0d5b-105">**MoveFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0d5b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a0d5b-106">Attributes and elements</span></span>

<span data-ttu-id="a0d5b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a0d5b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0d5b-108">属性</span><span class="sxs-lookup"><span data-stu-id="a0d5b-108">Attributes</span></span>

<span data-ttu-id="a0d5b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a0d5b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0d5b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a0d5b-110">Child elements</span></span>

|<span data-ttu-id="a0d5b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a0d5b-111">**Element**</span></span>|<span data-ttu-id="a0d5b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a0d5b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0d5b-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a0d5b-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a0d5b-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="a0d5b-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a0d5b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="a0d5b-115">Parent elements</span></span>

<span data-ttu-id="a0d5b-116">なし。</span><span class="sxs-lookup"><span data-stu-id="a0d5b-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a0d5b-117">注釈</span><span class="sxs-lookup"><span data-stu-id="a0d5b-117">Remarks</span></span>

<span data-ttu-id="a0d5b-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a0d5b-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0d5b-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a0d5b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0d5b-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="a0d5b-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a0d5b-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a0d5b-121">Schema name</span></span>  <br/> |<span data-ttu-id="a0d5b-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a0d5b-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="a0d5b-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a0d5b-123">Validation file</span></span>  <br/> |<span data-ttu-id="a0d5b-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a0d5b-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a0d5b-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a0d5b-125">Can be empty</span></span>  <br/> |<span data-ttu-id="a0d5b-126">いいえ</span><span class="sxs-lookup"><span data-stu-id="a0d5b-126">False</span></span>  <br/> |
   

