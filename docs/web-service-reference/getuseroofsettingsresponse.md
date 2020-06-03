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
description: GetUserOofSettingsResponse 要素には、応答メッセージと、ユーザーの不在時 (OOF) の設定が含まれています。
ms.openlocfilehash: f7f28c67fd36630ffb5294ab35c0fef2f467ba22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457817"
---
# <a name="getuseroofsettingsresponse"></a><span data-ttu-id="73991-103">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="73991-103">GetUserOofSettingsResponse</span></span>

<span data-ttu-id="73991-104">**Getuseroofsettingsresponse**要素には、応答メッセージと、ユーザーの不在時 (OOF) の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="73991-104">The **GetUserOofSettingsResponse** element contains the response message and the Out of Office (OOF) settings for a user.</span></span> 
  
```xml
<GetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
   <OofSettings>...</OofSettings>
   <AllowExternalOof>...</AllowExternalOof>
</GetUserOofSettingsResponse>
```

 <span data-ttu-id="73991-105">**GetUserOofSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="73991-105">**GetUserOofSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73991-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="73991-106">Attributes and elements</span></span>

<span data-ttu-id="73991-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="73991-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73991-108">属性</span><span class="sxs-lookup"><span data-stu-id="73991-108">Attributes</span></span>

<span data-ttu-id="73991-109">なし。</span><span class="sxs-lookup"><span data-stu-id="73991-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73991-110">子要素</span><span class="sxs-lookup"><span data-stu-id="73991-110">Child elements</span></span>

|<span data-ttu-id="73991-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="73991-111">**Element**</span></span>|<span data-ttu-id="73991-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="73991-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73991-113">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="73991-113">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="73991-114">応答状態に関する説明情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="73991-114">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="73991-115">OofSettings</span><span class="sxs-lookup"><span data-stu-id="73991-115">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="73991-116">不在時の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="73991-116">Contains the OOF settings.</span></span>  <br/> |
|[<span data-ttu-id="73991-117">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="73991-117">AllowExternalOof</span></span>](allowexternaloof.md) <br/> |<span data-ttu-id="73991-118">外部の OOF メッセージが送信されるユーザーを識別する値を格納します。</span><span class="sxs-lookup"><span data-stu-id="73991-118">Contains a value that identifies to whom external OOF messages are sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="73991-119">親要素</span><span class="sxs-lookup"><span data-stu-id="73991-119">Parent elements</span></span>

<span data-ttu-id="73991-120">なし。</span><span class="sxs-lookup"><span data-stu-id="73991-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="73991-121">注釈</span><span class="sxs-lookup"><span data-stu-id="73991-121">Remarks</span></span>

<span data-ttu-id="73991-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="73991-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73991-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="73991-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73991-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="73991-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="73991-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="73991-125">Schema Name</span></span>  <br/> |<span data-ttu-id="73991-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="73991-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="73991-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="73991-127">Validation File</span></span>  <br/> |<span data-ttu-id="73991-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="73991-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="73991-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="73991-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="73991-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="73991-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73991-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="73991-131">See also</span></span>



[<span data-ttu-id="73991-132">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="73991-132">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="73991-133">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="73991-133">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

