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
description: InternalReply 要素には、ユーザーのドメインまたは信頼されたドメイン内の他のユーザーに送信される不在 (OOF) 応答が含まれています。
ms.openlocfilehash: 24c278ebd3acf83e87fbf72650eb3d5d438d5c22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465584"
---
# <a name="internalreply"></a><span data-ttu-id="f9dc5-103">InternalReply</span><span class="sxs-lookup"><span data-stu-id="f9dc5-103">InternalReply</span></span>

<span data-ttu-id="f9dc5-104">**Internalreply**要素には、ユーザーのドメインまたは信頼されたドメイン内の他のユーザーに送信される不在 (OOF) 応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f9dc5-104">The **InternalReply** element contains the out of office (OOF) response sent to other users in the user's domain or trusted domains.</span></span> 
  
```XML
<InternalReply>
   <Message/> 
</InternalReply>
```

 <span data-ttu-id="f9dc5-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="f9dc5-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9dc5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f9dc5-106">Attributes and elements</span></span>

<span data-ttu-id="f9dc5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f9dc5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9dc5-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9dc5-108">Attributes</span></span>

|<span data-ttu-id="f9dc5-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="f9dc5-109">**Attribute**</span></span>|<span data-ttu-id="f9dc5-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="f9dc5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f9dc5-111">xml: lang</span><span class="sxs-lookup"><span data-stu-id="f9dc5-111">xml:lang</span></span>  <br/> |<span data-ttu-id="f9dc5-112">**Internalreply**メッセージで使用される言語を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9dc5-112">Specifies the language used in the **InternalReply** message.</span></span> <span data-ttu-id="f9dc5-113">この属性に指定できる値は、IETF RFC 3066 で定義されています。</span><span class="sxs-lookup"><span data-stu-id="f9dc5-113">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f9dc5-114">子要素</span><span class="sxs-lookup"><span data-stu-id="f9dc5-114">Child elements</span></span>

|<span data-ttu-id="f9dc5-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="f9dc5-115">**Element**</span></span>|<span data-ttu-id="f9dc5-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="f9dc5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9dc5-117">メッセージ (可用性)</span><span class="sxs-lookup"><span data-stu-id="f9dc5-117">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="f9dc5-118">OOF 応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="f9dc5-118">Contains the OOF response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f9dc5-119">親要素</span><span class="sxs-lookup"><span data-stu-id="f9dc5-119">Parent elements</span></span>

|<span data-ttu-id="f9dc5-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="f9dc5-120">**Element**</span></span>|<span data-ttu-id="f9dc5-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="f9dc5-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9dc5-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="f9dc5-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="f9dc5-123">OOF 設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9dc5-123">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="f9dc5-124">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f9dc5-124">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="f9dc5-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="f9dc5-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="f9dc5-126">不在時の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="f9dc5-126">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="f9dc5-127">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f9dc5-127">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f9dc5-128">注釈</span><span class="sxs-lookup"><span data-stu-id="f9dc5-128">Remarks</span></span>

<span data-ttu-id="f9dc5-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f9dc5-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="f9dc5-130">例</span><span class="sxs-lookup"><span data-stu-id="f9dc5-130">Example</span></span>

<span data-ttu-id="f9dc5-131">SetUserOofSettings 要求の次の例では、 [Oofstate](oofstate.md)を**有効**に設定し、不在時の時間を10日間に設定し、内部および外部の oof メッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="f9dc5-131">The following example of a SetUserOofSettings request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="f9dc5-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f9dc5-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9dc5-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="f9dc5-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9dc5-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f9dc5-134">Schema Name</span></span>  <br/> |<span data-ttu-id="f9dc5-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f9dc5-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="f9dc5-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f9dc5-136">Validation File</span></span>  <br/> |<span data-ttu-id="f9dc5-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f9dc5-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9dc5-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f9dc5-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="f9dc5-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="f9dc5-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9dc5-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="f9dc5-140">See also</span></span>



[<span data-ttu-id="f9dc5-141">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="f9dc5-141">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="f9dc5-142">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="f9dc5-142">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

