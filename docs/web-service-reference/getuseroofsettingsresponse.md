---
title: GetUserOofSettingsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettingsResponse
api_type:
- schema
ms.assetid: 011cb38b-da3c-4b1b-8836-a6b212b511f6
description: GetUserOofSettingsResponse 要素には、応答メッセージと、ユーザーの Office (OOF) の設定が含まれています。
ms.openlocfilehash: dc63b6d54471973ce5961a5a5ad6a23f6521fc0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831693"
---
# <a name="getuseroofsettingsresponse"></a><span data-ttu-id="188e7-103">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="188e7-103">GetUserOofSettingsResponse</span></span>

<span data-ttu-id="188e7-104">**GetUserOofSettingsResponse**要素には、応答メッセージと、ユーザーの Office (OOF) の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="188e7-104">The **GetUserOofSettingsResponse** element contains the response message and the Out of Office (OOF) settings for a user.</span></span> 
  
```xml
<GetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
   <OofSettings>...</OofSettings>
   <AllowExternalOof>...</AllowExternalOof>
</GetUserOofSettingsResponse>
```

 <span data-ttu-id="188e7-105">**GetUserOofSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="188e7-105">**GetUserOofSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="188e7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="188e7-106">Attributes and elements</span></span>

<span data-ttu-id="188e7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="188e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="188e7-108">属性</span><span class="sxs-lookup"><span data-stu-id="188e7-108">Attributes</span></span>

<span data-ttu-id="188e7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="188e7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="188e7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="188e7-110">Child elements</span></span>

|<span data-ttu-id="188e7-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="188e7-111">**Element**</span></span>|<span data-ttu-id="188e7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="188e7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="188e7-113">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="188e7-113">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="188e7-114">応答ステータスに関する説明情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="188e7-114">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="188e7-115">OofSettings</span><span class="sxs-lookup"><span data-stu-id="188e7-115">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="188e7-116">不在の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="188e7-116">Contains the OOF settings.</span></span>  <br/> |
|[<span data-ttu-id="188e7-117">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="188e7-117">AllowExternalOof</span></span>](allowexternaloof.md) <br/> |<span data-ttu-id="188e7-118">外部の OOF メッセージを送信するを識別する値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="188e7-118">Contains a value that identifies to whom external OOF messages are sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="188e7-119">親要素</span><span class="sxs-lookup"><span data-stu-id="188e7-119">Parent elements</span></span>

<span data-ttu-id="188e7-120">なし。</span><span class="sxs-lookup"><span data-stu-id="188e7-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="188e7-121">備考</span><span class="sxs-lookup"><span data-stu-id="188e7-121">Remarks</span></span>

<span data-ttu-id="188e7-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="188e7-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="188e7-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="188e7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="188e7-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="188e7-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="188e7-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="188e7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="188e7-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="188e7-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="188e7-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="188e7-127">Validation File</span></span>  <br/> |<span data-ttu-id="188e7-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="188e7-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="188e7-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="188e7-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="188e7-130">False</span><span class="sxs-lookup"><span data-stu-id="188e7-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="188e7-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="188e7-131">See also</span></span>



[<span data-ttu-id="188e7-132">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="188e7-132">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="188e7-133">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="188e7-133">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

