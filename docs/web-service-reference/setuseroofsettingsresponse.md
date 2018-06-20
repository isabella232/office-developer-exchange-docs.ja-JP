---
title: SetUserOofSettingsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettingsResponse
api_type:
- schema
ms.assetid: 8aa4025b-38df-4d63-a6a5-c3b932bec26e
description: SetUserOofSettingsResponse 要素には、SetUserOofSettingsRequest メッセージの試行の結果が含まれています。
ms.openlocfilehash: ab2eaaad1b7b094baad724ec56f4c26280f1f15f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833471"
---
# <a name="setuseroofsettingsresponse"></a><span data-ttu-id="f4ecb-103">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="f4ecb-103">SetUserOofSettingsResponse</span></span>

<span data-ttu-id="f4ecb-104">**SetUserOofSettingsResponse**要素には、 [SetUserOofSettingsRequest](setuseroofsettingsrequest.md)メッセージの試行の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f4ecb-104">The **SetUserOofSettingsResponse** element contains the result of a [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) message attempt.</span></span> 
  
```xml
<SetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
<SetUserOofSettingsResponse>
```

 <span data-ttu-id="f4ecb-105">**SetUserOofSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="f4ecb-105">**SetUserOofSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4ecb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f4ecb-106">Attributes and elements</span></span>

<span data-ttu-id="f4ecb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f4ecb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4ecb-108">属性</span><span class="sxs-lookup"><span data-stu-id="f4ecb-108">Attributes</span></span>

<span data-ttu-id="f4ecb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f4ecb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4ecb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f4ecb-110">Child elements</span></span>

|<span data-ttu-id="f4ecb-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f4ecb-111">**Element**</span></span>|<span data-ttu-id="f4ecb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f4ecb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4ecb-113">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f4ecb-113">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="f4ecb-114">応答ステータスに関する説明情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f4ecb-114">Provides descriptive information about the response status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f4ecb-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f4ecb-115">Parent elements</span></span>

<span data-ttu-id="f4ecb-116">なし。</span><span class="sxs-lookup"><span data-stu-id="f4ecb-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f4ecb-117">備考</span><span class="sxs-lookup"><span data-stu-id="f4ecb-117">Remarks</span></span>

<span data-ttu-id="f4ecb-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="f4ecb-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4ecb-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="f4ecb-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4ecb-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="f4ecb-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f4ecb-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f4ecb-121">Schema Name</span></span>  <br/> |<span data-ttu-id="f4ecb-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f4ecb-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f4ecb-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f4ecb-123">Validation File</span></span>  <br/> |<span data-ttu-id="f4ecb-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f4ecb-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f4ecb-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f4ecb-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4ecb-126">False</span><span class="sxs-lookup"><span data-stu-id="f4ecb-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4ecb-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="f4ecb-127">See also</span></span>



[<span data-ttu-id="f4ecb-128">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="f4ecb-128">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

