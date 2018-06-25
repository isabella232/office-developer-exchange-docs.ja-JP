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
description: メールボックス要素では、メールボックス ユーザーを表すを SetUserOofSettings のか、GetUserOofSettings を要求します。
ms.openlocfilehash: 2e901ae0df56542f56f247184254294735018468
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832254"
---
# <a name="mailbox-availability"></a><span data-ttu-id="2d298-103">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="2d298-103">Mailbox (Availability)</span></span>

<span data-ttu-id="2d298-104">**メールボックス**要素では、メールボックス ユーザーを表すを SetUserOofSettings のか、GetUserOofSettings を要求します。</span><span class="sxs-lookup"><span data-stu-id="2d298-104">The **Mailbox** element represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span> 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

<span data-ttu-id="2d298-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="2d298-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2d298-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2d298-106">Attributes and elements</span></span>

<span data-ttu-id="2d298-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2d298-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d298-108">属性</span><span class="sxs-lookup"><span data-stu-id="2d298-108">Attributes</span></span>

<span data-ttu-id="2d298-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2d298-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d298-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2d298-110">Child elements</span></span>

|<span data-ttu-id="2d298-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2d298-111">**Element**</span></span>|<span data-ttu-id="2d298-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2d298-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d298-113">名 (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="2d298-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="2d298-114">メールボックス ユーザーの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="2d298-114">Represents the display name of the mailbox user.</span></span> <span data-ttu-id="2d298-115">この要素では、SetUserOofSettingsRequest では省略可能です。</span><span class="sxs-lookup"><span data-stu-id="2d298-115">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="2d298-116">GetUserOofSettingsRequest には、この要素が返されます。</span><span class="sxs-lookup"><span data-stu-id="2d298-116">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
|[<span data-ttu-id="2d298-117">アドレス (文字列)</span><span class="sxs-lookup"><span data-stu-id="2d298-117">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="2d298-118">メールボックス ユーザーの電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="2d298-118">Represents the e-mail address of the mailbox user.</span></span> <span data-ttu-id="2d298-119">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="2d298-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="2d298-120">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="2d298-120">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="2d298-121">メッセージのルーティング プロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="2d298-121">Represents the routing protocol for the message.</span></span> <span data-ttu-id="2d298-122">この要素では、SetUserOofSettingsRequest では省略可能です。</span><span class="sxs-lookup"><span data-stu-id="2d298-122">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="2d298-123">GetUserOofSettingsRequest には、この要素が返されます。</span><span class="sxs-lookup"><span data-stu-id="2d298-123">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d298-124">親要素</span><span class="sxs-lookup"><span data-stu-id="2d298-124">Parent elements</span></span>

|<span data-ttu-id="2d298-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="2d298-125">**Element**</span></span>|<span data-ttu-id="2d298-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="2d298-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d298-127">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="2d298-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md) <br/> |<span data-ttu-id="2d298-128">メールボックス ユーザーの Office (OOF) の設定とメッセージの取得に使用されます。</span><span class="sxs-lookup"><span data-stu-id="2d298-128">Used to get a mailbox user's Out of Office (OOF) settings and messages.</span></span>  <br/> <span data-ttu-id="2d298-129">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="2d298-129">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[<span data-ttu-id="2d298-130">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="2d298-130">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="2d298-131">メールボックス ユーザーの不在時の設定とメッセージの設定に使用されます。</span><span class="sxs-lookup"><span data-stu-id="2d298-131">Used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="2d298-132">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="2d298-132">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2d298-133">備考</span><span class="sxs-lookup"><span data-stu-id="2d298-133">Remarks</span></span>

<span data-ttu-id="2d298-134">電子メール アドレスを使用して、不在時の設定が含まれている予定表フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="2d298-134">The e-mail address is used to identify the calendar folder that contains the OOF settings.</span></span> 
  
<span data-ttu-id="2d298-135">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="2d298-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d298-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="2d298-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d298-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="2d298-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2d298-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2d298-138">Schema Name</span></span>  <br/> |<span data-ttu-id="2d298-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2d298-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="2d298-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2d298-140">Validation File</span></span>  <br/> |<span data-ttu-id="2d298-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2d298-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2d298-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2d298-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="2d298-143">False</span><span class="sxs-lookup"><span data-stu-id="2d298-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d298-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="2d298-144">See also</span></span>

- [<span data-ttu-id="2d298-145">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="2d298-145">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="2d298-146">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="2d298-146">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

