---
title: ExternalAudience
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExternalAudience
api_type:
- schema
ms.assetid: 79dc2a4c-f7dd-46d1-8f31-149116e1f76e
description: ExternalAudience 要素は、外部不在 (OOF) メッセージが送信されるユーザーを決定する値を設定または格納します。
ms.openlocfilehash: b3fcebd9042b07bb9a8294196799ef2a13d78bdd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530601"
---
# <a name="externalaudience"></a><span data-ttu-id="61cb5-103">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="61cb5-103">ExternalAudience</span></span>

<span data-ttu-id="61cb5-104">**Externalaudience**要素は、外部不在 (OOF) メッセージが送信されるユーザーを決定する値を設定または格納します。</span><span class="sxs-lookup"><span data-stu-id="61cb5-104">The **ExternalAudience** element sets or contains a value that determines to whom external Out of Office (OOF) messages are sent.</span></span> 
  
```xml
<ExternalAudience>None or Known or All</ExternalAudience>
```

 <span data-ttu-id="61cb5-105">**ExternalAudience**</span><span class="sxs-lookup"><span data-stu-id="61cb5-105">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61cb5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="61cb5-106">Attributes and elements</span></span>

<span data-ttu-id="61cb5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="61cb5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61cb5-108">属性</span><span class="sxs-lookup"><span data-stu-id="61cb5-108">Attributes</span></span>

<span data-ttu-id="61cb5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="61cb5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61cb5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="61cb5-110">Child elements</span></span>

<span data-ttu-id="61cb5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="61cb5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="61cb5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="61cb5-112">Parent elements</span></span>

|<span data-ttu-id="61cb5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="61cb5-113">**Element**</span></span>|<span data-ttu-id="61cb5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="61cb5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61cb5-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="61cb5-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="61cb5-116">OOF 設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="61cb5-116">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="61cb5-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="61cb5-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="61cb5-118">OofSettings</span><span class="sxs-lookup"><span data-stu-id="61cb5-118">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="61cb5-119">不在時の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="61cb5-119">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="61cb5-120">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="61cb5-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="61cb5-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="61cb5-121">Text value</span></span>

<span data-ttu-id="61cb5-122">この要素にはテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="61cb5-122">A text value is required for this element.</span></span> <span data-ttu-id="61cb5-123">次の表に、この要素で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="61cb5-123">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="61cb5-124">**値**</span><span class="sxs-lookup"><span data-stu-id="61cb5-124">**Value**</span></span>|<span data-ttu-id="61cb5-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="61cb5-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="61cb5-126">**なし**</span><span class="sxs-lookup"><span data-stu-id="61cb5-126">**None**</span></span> <br/> |<span data-ttu-id="61cb5-127">メールボックスユーザーの組織外の電子メール送信者は、ユーザーにメッセージを送信すると、外部の不在時メッセージ応答を受信しません。</span><span class="sxs-lookup"><span data-stu-id="61cb5-127">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="61cb5-128">**一般的**</span><span class="sxs-lookup"><span data-stu-id="61cb5-128">**Known**</span></span> <br/> |<span data-ttu-id="61cb5-129">メールボックスユーザーの組織外の電子メール送信者がユーザーにメッセージを送信すると、送信者がユーザーの Exchange ストアの連絡先リストにある場合にのみ、外部の OOF メッセージ応答が受信されます。</span><span class="sxs-lookup"><span data-stu-id="61cb5-129">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="61cb5-130">**All**</span><span class="sxs-lookup"><span data-stu-id="61cb5-130">**All**</span></span> <br/> |<span data-ttu-id="61cb5-131">メールボックスユーザーの組織外の電子メール送信者は、ユーザーにメッセージを送信すると、外部の OOF メッセージ応答を受信します。</span><span class="sxs-lookup"><span data-stu-id="61cb5-131">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="61cb5-132">注釈</span><span class="sxs-lookup"><span data-stu-id="61cb5-132">Remarks</span></span>

<span data-ttu-id="61cb5-133">この要素は、 [AllowExternalOof](allowexternaloof.md)要素と同じ型を共有します。</span><span class="sxs-lookup"><span data-stu-id="61cb5-133">This element shares the same type as the [AllowExternalOof](allowexternaloof.md) element.</span></span> 
  
<span data-ttu-id="61cb5-134">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="61cb5-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="61cb5-135">例</span><span class="sxs-lookup"><span data-stu-id="61cb5-135">Example</span></span>

<span data-ttu-id="61cb5-136">SetUserOofSettings 要求の次の例では、OoFState を**Enabled**に設定し、外部対象ユーザーを**すべて**に設定し、oof の時間を10日に設定し、内部および外部の oof メッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="61cb5-136">The following example of a SetUserOofSettings request sets the OoFState to **Enabled**, sets the external audience to **All**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
```
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

## <a name="element-information"></a><span data-ttu-id="61cb5-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="61cb5-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61cb5-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="61cb5-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61cb5-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="61cb5-139">Schema Name</span></span>  <br/> |<span data-ttu-id="61cb5-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="61cb5-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="61cb5-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="61cb5-141">Validation File</span></span>  <br/> |<span data-ttu-id="61cb5-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="61cb5-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="61cb5-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="61cb5-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="61cb5-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="61cb5-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61cb5-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="61cb5-145">See also</span></span>



[<span data-ttu-id="61cb5-146">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="61cb5-146">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="61cb5-147">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="61cb5-147">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

