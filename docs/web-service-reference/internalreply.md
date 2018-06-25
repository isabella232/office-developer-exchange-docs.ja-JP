---
title: InternalReply
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalReply
api_type:
- schema
ms.assetid: 1d784ded-b874-4eb1-8f6d-2e0e03330e1e
description: InternalReply 要素には、外出中 (OOF) 応答を送信するユーザーのドメインまたは信頼されるドメイン内の他のユーザーの出力が含まれています。
ms.openlocfilehash: ac5e9eadac7f45c233007ffb05f4d2430875ec52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831955"
---
# <a name="internalreply"></a><span data-ttu-id="e6157-103">InternalReply</span><span class="sxs-lookup"><span data-stu-id="e6157-103">InternalReply</span></span>

<span data-ttu-id="e6157-104">**InternalReply**要素には、外出中 (OOF) 応答を送信するユーザーのドメインまたは信頼されるドメイン内の他のユーザーの出力が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e6157-104">The **InternalReply** element contains the out of office (OOF) response sent to other users in the user's domain or trusted domains.</span></span> 
  
```XML
<InternalReply>
   <Message/> 
</InternalReply>
```

 <span data-ttu-id="e6157-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="e6157-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6157-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e6157-106">Attributes and elements</span></span>

<span data-ttu-id="e6157-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e6157-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6157-108">属性</span><span class="sxs-lookup"><span data-stu-id="e6157-108">Attributes</span></span>

|<span data-ttu-id="e6157-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="e6157-109">**Attribute**</span></span>|<span data-ttu-id="e6157-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="e6157-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e6157-111">xml:lang</span><span class="sxs-lookup"><span data-stu-id="e6157-111">xml:lang</span></span>  <br/> |<span data-ttu-id="e6157-112">**InternalReply**メッセージで使用される言語を指定します。</span><span class="sxs-lookup"><span data-stu-id="e6157-112">Specifies the language used in the **InternalReply** message.</span></span> <span data-ttu-id="e6157-113">この属性に指定できる値は、IETF RFC 3066 で定義されます。</span><span class="sxs-lookup"><span data-stu-id="e6157-113">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e6157-114">子要素</span><span class="sxs-lookup"><span data-stu-id="e6157-114">Child elements</span></span>

|<span data-ttu-id="e6157-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="e6157-115">**Element**</span></span>|<span data-ttu-id="e6157-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="e6157-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6157-117">メッセージ (可用性)</span><span class="sxs-lookup"><span data-stu-id="e6157-117">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="e6157-118">不在時の応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e6157-118">Contains the OOF response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e6157-119">親要素</span><span class="sxs-lookup"><span data-stu-id="e6157-119">Parent elements</span></span>

|<span data-ttu-id="e6157-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="e6157-120">**Element**</span></span>|<span data-ttu-id="e6157-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="e6157-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6157-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e6157-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="e6157-123">不在の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="e6157-123">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="e6157-124">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="e6157-124">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="e6157-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="e6157-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="e6157-126">不在の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e6157-126">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="e6157-127">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="e6157-127">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e6157-128">備考</span><span class="sxs-lookup"><span data-stu-id="e6157-128">Remarks</span></span>

<span data-ttu-id="e6157-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e6157-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="e6157-130">例</span><span class="sxs-lookup"><span data-stu-id="e6157-130">Example</span></span>

<span data-ttu-id="e6157-131">SetUserOofSettings 要求の次の使用例は、 [OofState](oofstate.md)を**有効**に設定、10 日間、不在時の期間を設定し、内部と外部の OOF メッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="e6157-131">The following example of a SetUserOofSettings request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="e6157-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="e6157-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6157-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="e6157-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e6157-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e6157-134">Schema Name</span></span>  <br/> |<span data-ttu-id="e6157-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e6157-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="e6157-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e6157-136">Validation File</span></span>  <br/> |<span data-ttu-id="e6157-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e6157-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e6157-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e6157-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="e6157-139">False</span><span class="sxs-lookup"><span data-stu-id="e6157-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6157-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="e6157-140">See also</span></span>



[<span data-ttu-id="e6157-141">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="e6157-141">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="e6157-142">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="e6157-142">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

