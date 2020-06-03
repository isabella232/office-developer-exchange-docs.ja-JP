---
title: メールボックス (可用性)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: affd192e-8914-473f-9098-d9bdf898de2c
description: Mailbox 要素は、SetUserOofSettings または GetUserOofSettings 要求のメールボックスユーザーを表します。
ms.openlocfilehash: 1bda6e8b90551b86b4e1c2711ac25693a65e5410
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458076"
---
# <a name="mailbox-availability"></a><span data-ttu-id="373b0-103">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="373b0-103">Mailbox (Availability)</span></span>

<span data-ttu-id="373b0-104">**Mailbox**要素は、SetUserOofSettings または getuseroofsettings 要求のメールボックスユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="373b0-104">The **Mailbox** element represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span> 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

<span data-ttu-id="373b0-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="373b0-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="373b0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="373b0-106">Attributes and elements</span></span>

<span data-ttu-id="373b0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="373b0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="373b0-108">属性</span><span class="sxs-lookup"><span data-stu-id="373b0-108">Attributes</span></span>

<span data-ttu-id="373b0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="373b0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="373b0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="373b0-110">Child elements</span></span>

|<span data-ttu-id="373b0-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="373b0-111">**Element**</span></span>|<span data-ttu-id="373b0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="373b0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="373b0-113">Name (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="373b0-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="373b0-114">メールボックスユーザーの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="373b0-114">Represents the display name of the mailbox user.</span></span> <span data-ttu-id="373b0-115">この要素は、SetUserOofSettingsRequest では省略可能です。</span><span class="sxs-lookup"><span data-stu-id="373b0-115">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="373b0-116">GetUserOofSettingsRequest は、この要素を返します。</span><span class="sxs-lookup"><span data-stu-id="373b0-116">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
|[<span data-ttu-id="373b0-117">Address (string)</span><span class="sxs-lookup"><span data-stu-id="373b0-117">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="373b0-118">メールボックスユーザーの電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="373b0-118">Represents the e-mail address of the mailbox user.</span></span> <span data-ttu-id="373b0-119">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="373b0-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="373b0-120">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="373b0-120">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="373b0-121">メッセージのルーティングプロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="373b0-121">Represents the routing protocol for the message.</span></span> <span data-ttu-id="373b0-122">この要素は、SetUserOofSettingsRequest では省略可能です。</span><span class="sxs-lookup"><span data-stu-id="373b0-122">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="373b0-123">GetUserOofSettingsRequest は、この要素を返します。</span><span class="sxs-lookup"><span data-stu-id="373b0-123">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="373b0-124">親要素</span><span class="sxs-lookup"><span data-stu-id="373b0-124">Parent elements</span></span>

|<span data-ttu-id="373b0-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="373b0-125">**Element**</span></span>|<span data-ttu-id="373b0-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="373b0-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="373b0-127">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="373b0-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md) <br/> |<span data-ttu-id="373b0-128">メールボックスユーザーの不在時 (OOF) の設定とメッセージを取得するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="373b0-128">Used to get a mailbox user's Out of Office (OOF) settings and messages.</span></span>  <br/> <span data-ttu-id="373b0-129">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="373b0-129">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[<span data-ttu-id="373b0-130">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="373b0-130">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="373b0-131">メールボックスユーザーの不在時の設定とメッセージを設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="373b0-131">Used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="373b0-132">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="373b0-132">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="373b0-133">注釈</span><span class="sxs-lookup"><span data-stu-id="373b0-133">Remarks</span></span>

<span data-ttu-id="373b0-134">この電子メールアドレスは、OOF 設定を含む予定表フォルダーを識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="373b0-134">The e-mail address is used to identify the calendar folder that contains the OOF settings.</span></span> 
  
<span data-ttu-id="373b0-135">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="373b0-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="373b0-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="373b0-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="373b0-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="373b0-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="373b0-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="373b0-138">Schema Name</span></span>  <br/> |<span data-ttu-id="373b0-139">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="373b0-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="373b0-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="373b0-140">Validation File</span></span>  <br/> |<span data-ttu-id="373b0-141">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="373b0-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="373b0-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="373b0-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="373b0-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="373b0-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="373b0-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="373b0-144">See also</span></span>

- [<span data-ttu-id="373b0-145">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="373b0-145">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="373b0-146">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="373b0-146">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

