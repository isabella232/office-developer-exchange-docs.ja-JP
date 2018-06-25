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
ms.openlocfilehash: 86630f39a7fb415ed57f280705f068eb50f0adb9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832487"
---
# <a name="movefolderresponse"></a><span data-ttu-id="dcd51-103">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="dcd51-103">MoveFolderResponse</span></span>

<span data-ttu-id="dcd51-104">**MoveFolderResponse**要素は、MoveFolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="dcd51-104">The **MoveFolderResponse** element defines a response to a MoveFolder request.</span></span> 
  
```xml
<MoveFolderResponse>
   <ResponseMessages/>
</MoveFolderResponse>
```

 <span data-ttu-id="dcd51-105">**MoveFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="dcd51-105">**MoveFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dcd51-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dcd51-106">Attributes and elements</span></span>

<span data-ttu-id="dcd51-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dcd51-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dcd51-108">属性</span><span class="sxs-lookup"><span data-stu-id="dcd51-108">Attributes</span></span>

<span data-ttu-id="dcd51-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dcd51-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dcd51-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dcd51-110">Child elements</span></span>

|<span data-ttu-id="dcd51-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="dcd51-111">**Element**</span></span>|<span data-ttu-id="dcd51-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dcd51-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcd51-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dcd51-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="dcd51-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="dcd51-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dcd51-115">親要素</span><span class="sxs-lookup"><span data-stu-id="dcd51-115">Parent elements</span></span>

<span data-ttu-id="dcd51-116">なし。</span><span class="sxs-lookup"><span data-stu-id="dcd51-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dcd51-117">備考</span><span class="sxs-lookup"><span data-stu-id="dcd51-117">Remarks</span></span>

<span data-ttu-id="dcd51-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="dcd51-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dcd51-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="dcd51-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dcd51-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="dcd51-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dcd51-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dcd51-121">Schema name</span></span>  <br/> |<span data-ttu-id="dcd51-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="dcd51-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="dcd51-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dcd51-123">Validation file</span></span>  <br/> |<span data-ttu-id="dcd51-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dcd51-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dcd51-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="dcd51-125">Can be empty</span></span>  <br/> |<span data-ttu-id="dcd51-126">いいえ</span><span class="sxs-lookup"><span data-stu-id="dcd51-126">False</span></span>  <br/> |
   

