---
title: OofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofSettings
api_type:
- schema
ms.assetid: 8f37d174-db11-427c-bbed-fdde754a60c7
description: OofSettings 要素には、不在 (OOF) の設定が含まれています。
ms.openlocfilehash: c1b214fd8bfab5b7a82d41a5187cf6e0fc4ba79c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467194"
---
# <a name="oofsettings"></a><span data-ttu-id="d75db-103">OofSettings</span><span class="sxs-lookup"><span data-stu-id="d75db-103">OofSettings</span></span>

<span data-ttu-id="d75db-104">**Oofsettings**要素には、不在 (OOF) の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d75db-104">The **OofSettings** element contains the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="d75db-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="d75db-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
[<span data-ttu-id="d75db-106">OofSettings</span><span class="sxs-lookup"><span data-stu-id="d75db-106">OofSettings</span></span>](oofsettings.md)
  
```xml
<OofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</OofSettings>
```

 <span data-ttu-id="d75db-107">**UserOofSettings**</span><span class="sxs-lookup"><span data-stu-id="d75db-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d75db-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d75db-108">Attributes and elements</span></span>

<span data-ttu-id="d75db-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d75db-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d75db-110">属性</span><span class="sxs-lookup"><span data-stu-id="d75db-110">Attributes</span></span>

<span data-ttu-id="d75db-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d75db-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d75db-112">子要素</span><span class="sxs-lookup"><span data-stu-id="d75db-112">Child elements</span></span>

|<span data-ttu-id="d75db-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="d75db-113">**Element**</span></span>|<span data-ttu-id="d75db-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d75db-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d75db-115">OofState</span><span class="sxs-lookup"><span data-stu-id="d75db-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="d75db-116">ユーザーの不在時の状態を格納します。</span><span class="sxs-lookup"><span data-stu-id="d75db-116">Contains the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="d75db-117">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="d75db-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="d75db-118">外部の OOF メッセージが送信されるユーザーを決定する値を格納します。</span><span class="sxs-lookup"><span data-stu-id="d75db-118">Contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="d75db-119">Duration (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="d75db-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="d75db-120">[Oofstate](oofstate.md)要素が [**スケジュール済み**] に設定されている場合に、OOF の状態が有効になる期間を含みます。</span><span class="sxs-lookup"><span data-stu-id="d75db-120">Contains the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="d75db-121">[Oofstate](oofstate.md)要素が**Enabled**または**Disabled**に設定されている場合、この要素の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="d75db-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="d75db-122">InternalReply</span><span class="sxs-lookup"><span data-stu-id="d75db-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="d75db-123">ユーザーのドメインまたは信頼されたドメイン内の他のユーザーに送信される OOF 応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="d75db-123">Contains the OOF response sent to other users in the user's domain or trusted domain.</span></span>  <br/> |
|[<span data-ttu-id="d75db-124">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="d75db-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="d75db-125">受信者のドメインまたは信頼されたドメイン外のアドレスに送信される OOF 応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="d75db-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d75db-126">親要素</span><span class="sxs-lookup"><span data-stu-id="d75db-126">Parent elements</span></span>

|<span data-ttu-id="d75db-127">**要素**</span><span class="sxs-lookup"><span data-stu-id="d75db-127">**Element**</span></span>|<span data-ttu-id="d75db-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="d75db-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d75db-129">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="d75db-129">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="d75db-130">応答結果とユーザーの OOF 設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d75db-130">Contains the response results and the OOF settings for a user.</span></span>  <br/> <span data-ttu-id="d75db-131">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d75db-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d75db-132">注釈</span><span class="sxs-lookup"><span data-stu-id="d75db-132">Remarks</span></span>

<span data-ttu-id="d75db-133">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d75db-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d75db-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d75db-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d75db-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="d75db-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d75db-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d75db-136">Schema Name</span></span>  <br/> |<span data-ttu-id="d75db-137">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d75db-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d75db-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d75db-138">Validation File</span></span>  <br/> |<span data-ttu-id="d75db-139">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d75db-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d75db-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d75db-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="d75db-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="d75db-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d75db-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="d75db-142">See also</span></span>



[<span data-ttu-id="d75db-143">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="d75db-143">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="d75db-144">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="d75db-144">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

