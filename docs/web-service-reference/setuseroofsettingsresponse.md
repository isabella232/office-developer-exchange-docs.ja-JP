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
description: SetUserOofSettingsResponse 要素には、Setuseroofsettingsresponse 要求メッセージの試行の結果が含まれています。
ms.openlocfilehash: 9b02d905f82488965f5ae0514a52eb6062aaff7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466130"
---
# <a name="setuseroofsettingsresponse"></a><span data-ttu-id="0ea52-103">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="0ea52-103">SetUserOofSettingsResponse</span></span>

<span data-ttu-id="0ea52-104">**Setuseroofsettingsresponse**要素には、 [Setuseroofsettingsresponse 要求](setuseroofsettingsrequest.md)メッセージの試行の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0ea52-104">The **SetUserOofSettingsResponse** element contains the result of a [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) message attempt.</span></span> 
  
```xml
<SetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
<SetUserOofSettingsResponse>
```

 <span data-ttu-id="0ea52-105">**SetUserOofSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="0ea52-105">**SetUserOofSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ea52-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0ea52-106">Attributes and elements</span></span>

<span data-ttu-id="0ea52-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0ea52-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ea52-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ea52-108">Attributes</span></span>

<span data-ttu-id="0ea52-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0ea52-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ea52-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0ea52-110">Child elements</span></span>

|<span data-ttu-id="0ea52-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="0ea52-111">**Element**</span></span>|<span data-ttu-id="0ea52-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0ea52-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ea52-113">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0ea52-113">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="0ea52-114">応答状態に関する説明情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0ea52-114">Provides descriptive information about the response status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ea52-115">親要素</span><span class="sxs-lookup"><span data-stu-id="0ea52-115">Parent elements</span></span>

<span data-ttu-id="0ea52-116">なし。</span><span class="sxs-lookup"><span data-stu-id="0ea52-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ea52-117">注釈</span><span class="sxs-lookup"><span data-stu-id="0ea52-117">Remarks</span></span>

<span data-ttu-id="0ea52-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0ea52-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ea52-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0ea52-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ea52-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="0ea52-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0ea52-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0ea52-121">Schema Name</span></span>  <br/> |<span data-ttu-id="0ea52-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0ea52-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0ea52-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0ea52-123">Validation File</span></span>  <br/> |<span data-ttu-id="0ea52-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0ea52-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0ea52-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0ea52-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ea52-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="0ea52-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ea52-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="0ea52-127">See also</span></span>



[<span data-ttu-id="0ea52-128">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="0ea52-128">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

