---
title: メッセージ (可用性)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Message
api_type:
- schema
ms.assetid: 1eec24dd-c981-41f4-a2f0-c51d43f1d7c0
description: メッセージ要素には、Office (OOF) の応答の出力が含まれています。
ms.openlocfilehash: 9facd04767fdcc0fd9dfd84fc6badb1a7633d2b5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832452"
---
# <a name="message-availability"></a><span data-ttu-id="8b9f0-103">メッセージ (可用性)</span><span class="sxs-lookup"><span data-stu-id="8b9f0-103">Message (Availability)</span></span>

<span data-ttu-id="8b9f0-104">**メッセージ**要素には、Office (OOF) の応答の出力が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8b9f0-104">The **Message** element contains the out of Office (OOF) response.</span></span> 
  
```xml
<Message/> 
```

 <span data-ttu-id="8b9f0-105">**string**</span><span class="sxs-lookup"><span data-stu-id="8b9f0-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b9f0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8b9f0-106">Attributes and elements</span></span>

<span data-ttu-id="8b9f0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8b9f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b9f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="8b9f0-108">Attributes</span></span>

<span data-ttu-id="8b9f0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8b9f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b9f0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8b9f0-110">Child elements</span></span>

<span data-ttu-id="8b9f0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8b9f0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8b9f0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8b9f0-112">Parent elements</span></span>

|<span data-ttu-id="8b9f0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8b9f0-113">**Element**</span></span>|<span data-ttu-id="8b9f0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8b9f0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b9f0-115">InternalReply</span><span class="sxs-lookup"><span data-stu-id="8b9f0-115">InternalReply</span></span>](internalreply.md) <br/> | <span data-ttu-id="8b9f0-116">送信者のドメインの他のユーザーに送信される不在時のメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8b9f0-116">Contains the OOF message sent to other users in the sender's domain.</span></span> <br/> <br/>  <span data-ttu-id="8b9f0-117">この要素に使用可能な XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="8b9f0-117">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/InternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/InternalReply` <br/> |
|[<span data-ttu-id="8b9f0-118">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="8b9f0-118">ExternalReply</span></span>](externalreply.md) <br/> | <span data-ttu-id="8b9f0-119">送信者のドメインの外部アドレスに送信される不在時のメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8b9f0-119">Contains the OOF message that is sent to addresses outside the sender's domain.</span></span>  <br/> <br/> <span data-ttu-id="8b9f0-120">この要素に使用可能な XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="8b9f0-120">The following are the possible XPath expressions to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/ExternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/ExternalReply` <br/> |
|[<span data-ttu-id="8b9f0-121">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="8b9f0-121">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="8b9f0-122">不在時のメッセージと、メッセージに使用する言語が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8b9f0-122">Contains an OOF message and the language used for the message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8b9f0-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8b9f0-123">Text value</span></span>

<span data-ttu-id="8b9f0-124">OOF メッセージを設定するのには、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="8b9f0-124">A text value is required to set the OOF message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8b9f0-125">備考</span><span class="sxs-lookup"><span data-stu-id="8b9f0-125">Remarks</span></span>

<span data-ttu-id="8b9f0-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8b9f0-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="8b9f0-127">例</span><span class="sxs-lookup"><span data-stu-id="8b9f0-127">Example</span></span>

<span data-ttu-id="8b9f0-128">[SetUserOofSettings 操作](setuseroofsettings-operation.md)要求の次の使用例は、 [OofState](oofstate.md)を**有効**に設定、不在時の期間を 10 日に設定し、内部と外部の OOF メッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="8b9f0-128">The following example of a [SetUserOofSettings operation](setuseroofsettings-operation.md) request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="8b9f0-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="8b9f0-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b9f0-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="8b9f0-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b9f0-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8b9f0-131">Schema Name</span></span>  <br/> |<span data-ttu-id="8b9f0-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8b9f0-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b9f0-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8b9f0-133">Validation File</span></span>  <br/> |<span data-ttu-id="8b9f0-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8b9f0-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b9f0-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8b9f0-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="8b9f0-136">False</span><span class="sxs-lookup"><span data-stu-id="8b9f0-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b9f0-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="8b9f0-137">See also</span></span>

- [<span data-ttu-id="8b9f0-138">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="8b9f0-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="8b9f0-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8b9f0-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

