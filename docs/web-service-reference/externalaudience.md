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
description: ExternalAudience 要素を設定または外部の Office (OOF) メッセージを送信するかを決定する値が含まれています。
ms.openlocfilehash: 836b0f6a5140a37e1584f571cb8e26534fe7a25f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760426"
---
# <a name="externalaudience"></a><span data-ttu-id="8d356-103">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="8d356-103">ExternalAudience</span></span>

<span data-ttu-id="8d356-104">**ExternalAudience**要素を設定または外部の Office (OOF) メッセージを送信するかを決定する値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8d356-104">The **ExternalAudience** element sets or contains a value that determines to whom external Out of Office (OOF) messages are sent.</span></span> 
  
```xml
<ExternalAudience>None or Known or All</ExternalAudience>
```

 <span data-ttu-id="8d356-105">**ExternalAudience**</span><span class="sxs-lookup"><span data-stu-id="8d356-105">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d356-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8d356-106">Attributes and elements</span></span>

<span data-ttu-id="8d356-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8d356-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d356-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d356-108">Attributes</span></span>

<span data-ttu-id="8d356-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8d356-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d356-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8d356-110">Child elements</span></span>

<span data-ttu-id="8d356-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8d356-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d356-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8d356-112">Parent elements</span></span>

|<span data-ttu-id="8d356-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8d356-113">**Element**</span></span>|<span data-ttu-id="8d356-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8d356-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d356-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="8d356-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="8d356-116">不在の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d356-116">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="8d356-117">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="8d356-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="8d356-118">OofSettings</span><span class="sxs-lookup"><span data-stu-id="8d356-118">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="8d356-119">不在の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8d356-119">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="8d356-120">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="8d356-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d356-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8d356-121">Text value</span></span>

<span data-ttu-id="8d356-122">テキスト値は、この要素の必要があります。</span><span class="sxs-lookup"><span data-stu-id="8d356-122">A text value is required for this element.</span></span> <span data-ttu-id="8d356-123">次の表は、この要素の有効な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="8d356-123">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="8d356-124">**値**</span><span class="sxs-lookup"><span data-stu-id="8d356-124">**Value**</span></span>|<span data-ttu-id="8d356-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="8d356-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8d356-126">**None**</span><span class="sxs-lookup"><span data-stu-id="8d356-126">**None**</span></span> <br/> |<span data-ttu-id="8d356-127">メールボックス ユーザーの組織外のユーザーにメッセージを送信するメールの送信者は、外部の OOF メッセージの応答を受信しません。</span><span class="sxs-lookup"><span data-stu-id="8d356-127">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="8d356-128">**呼ばれる**</span><span class="sxs-lookup"><span data-stu-id="8d356-128">**Known**</span></span> <br/> |<span data-ttu-id="8d356-129">メールボックス ユーザーの組織の外部ユーザーへのメッセージのみが表示されます、外部の OOF メッセージ応答送信者がユーザーの Exchange の場合に送信したメールの送信者は、連絡先リストを保存します。</span><span class="sxs-lookup"><span data-stu-id="8d356-129">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="8d356-130">**All**</span><span class="sxs-lookup"><span data-stu-id="8d356-130">**All**</span></span> <br/> |<span data-ttu-id="8d356-131">メールボックス ユーザーの組織外のユーザーにメッセージを送信するメールの送信者が外部の OOF メッセージの応答を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="8d356-131">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8d356-132">備考</span><span class="sxs-lookup"><span data-stu-id="8d356-132">Remarks</span></span>

<span data-ttu-id="8d356-133">この要素は、 [AllowExternalOof](allowexternaloof.md)要素と同じ型を共有します。</span><span class="sxs-lookup"><span data-stu-id="8d356-133">This element shares the same type as the [AllowExternalOof](allowexternaloof.md) element.</span></span> 
  
<span data-ttu-id="8d356-134">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="8d356-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="8d356-135">例</span><span class="sxs-lookup"><span data-stu-id="8d356-135">Example</span></span>

<span data-ttu-id="8d356-136">SetUserOofSettings 要求の次の使用例、OoFState を**有効**に設定に**すべて**の外部の対象ユーザーの設定、不在時の期間を 10 日に設定、内部と外部の OOF メッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="8d356-136">The following example of a SetUserOofSettings request sets the OoFState to **Enabled**, sets the external audience to **All**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
```
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

## <a name="element-information"></a><span data-ttu-id="8d356-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="8d356-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d356-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="8d356-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d356-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8d356-139">Schema Name</span></span>  <br/> |<span data-ttu-id="8d356-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8d356-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d356-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8d356-141">Validation File</span></span>  <br/> |<span data-ttu-id="8d356-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8d356-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d356-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8d356-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d356-144">False</span><span class="sxs-lookup"><span data-stu-id="8d356-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d356-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="8d356-145">See also</span></span>



[<span data-ttu-id="8d356-146">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="8d356-146">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="8d356-147">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="8d356-147">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

