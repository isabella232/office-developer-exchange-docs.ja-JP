---
title: UserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserOofSettings
api_type:
- schema
ms.assetid: 0a95ca63-660e-4cc0-82e4-3f74fb4ae21c
description: UserOofSettings 要素は、Office (OOF) の設定を指定します。
ms.openlocfilehash: a035fd89387ece632d83f5f72a564e4896bc6753
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839945"
---
# <a name="useroofsettings"></a><span data-ttu-id="81544-103">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="81544-103">UserOofSettings</span></span>

<span data-ttu-id="81544-104">**UserOofSettings**要素は、Office (OOF) の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="81544-104">The **UserOofSettings** element specifies the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="81544-105">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="81544-105">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
  
[<span data-ttu-id="81544-106">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="81544-106">UserOofSettings</span></span>](useroofsettings.md)
  
```xml
<UserOofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</UserOofSettings>
```

 <span data-ttu-id="81544-107">**UserOofSettings**</span><span class="sxs-lookup"><span data-stu-id="81544-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81544-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="81544-108">Attributes and elements</span></span>

<span data-ttu-id="81544-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="81544-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81544-110">属性</span><span class="sxs-lookup"><span data-stu-id="81544-110">Attributes</span></span>

<span data-ttu-id="81544-111">なし。</span><span class="sxs-lookup"><span data-stu-id="81544-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81544-112">子要素</span><span class="sxs-lookup"><span data-stu-id="81544-112">Child elements</span></span>

|<span data-ttu-id="81544-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="81544-113">**Element**</span></span>|<span data-ttu-id="81544-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="81544-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81544-115">OofState</span><span class="sxs-lookup"><span data-stu-id="81544-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="81544-116">ユーザーの不在時の状態を設定します。</span><span class="sxs-lookup"><span data-stu-id="81544-116">Sets the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="81544-117">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="81544-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="81544-118">設定または外部の OOF メッセージを送信するかを決定する値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="81544-118">Sets or contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="81544-119">期間 (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="81544-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="81544-120">不在の状態が有効である[OofState](oofstate.md)要素は、**スケジュール**に設定されている場合、期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="81544-120">Specifies the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="81544-121">[OofState](oofstate.md)要素は、**有効**または**無効**に設定されている場合、この要素の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="81544-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="81544-122">InternalReply</span><span class="sxs-lookup"><span data-stu-id="81544-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="81544-123">ユーザーのドメインまたは信頼されるドメイン内の他のユーザーに送信される不在時の応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="81544-123">Contains the OOF response sent to other users in the user's domain or trusted domains.</span></span>  <br/> |
|[<span data-ttu-id="81544-124">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="81544-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="81544-125">受信者のドメインまたは信頼されるドメインの外部アドレスに送信される不在時の応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="81544-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="81544-126">親要素</span><span class="sxs-lookup"><span data-stu-id="81544-126">Parent elements</span></span>

|<span data-ttu-id="81544-127">**要素**</span><span class="sxs-lookup"><span data-stu-id="81544-127">**Element**</span></span>|<span data-ttu-id="81544-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="81544-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81544-129">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="81544-129">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="81544-130">メールボックス ユーザーの不在時の設定とメッセージを設定するための引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="81544-130">Contains the arguments used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="81544-131">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="81544-131">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="81544-132">備考</span><span class="sxs-lookup"><span data-stu-id="81544-132">Remarks</span></span>

<span data-ttu-id="81544-133">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="81544-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="81544-134">例</span><span class="sxs-lookup"><span data-stu-id="81544-134">Example</span></span>

<span data-ttu-id="81544-135">SetUserOofSettings 要求の次の使用例は、OoFState を**有効**に設定、10 日間、不在時の期間を設定し、内部と外部の OOF メッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="81544-135">The following example of a SetUserOofSettings request sets the OoFState to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
```xml
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

## <a name="element-information"></a><span data-ttu-id="81544-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="81544-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81544-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="81544-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="81544-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="81544-138">Schema Name</span></span>  <br/> |<span data-ttu-id="81544-139">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="81544-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="81544-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="81544-140">Validation File</span></span>  <br/> |<span data-ttu-id="81544-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="81544-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="81544-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="81544-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="81544-143">False</span><span class="sxs-lookup"><span data-stu-id="81544-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81544-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="81544-144">See also</span></span>

- [<span data-ttu-id="81544-145">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="81544-145">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

