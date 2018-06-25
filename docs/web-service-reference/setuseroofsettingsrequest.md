---
title: SetUserOofSettingsRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettingsRequest
api_type:
- schema
ms.assetid: 628acf0b-3ebc-42f1-8ce2-7a02b4c8141f
description: SetUserOofSettingsRequest 要素には、メールボックスのユーザーの Office (OOF) の設定を設定するための引数が含まれています。
ms.openlocfilehash: ed54bb1d066da7b15605fb81931a6ef75dfc61bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833474"
---
# <a name="setuseroofsettingsrequest"></a><span data-ttu-id="f6553-103">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="f6553-103">SetUserOofSettingsRequest</span></span>

<span data-ttu-id="f6553-104">**SetUserOofSettingsRequest**要素には、メールボックスのユーザーの Office (OOF) の設定を設定するための引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f6553-104">The **SetUserOofSettingsRequest** element contains the arguments used to set a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<SetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
   <UserOofSettings>...</UserOofSettings>
<SetUserOofSettingsRequest>
```

 <span data-ttu-id="f6553-105">**SetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="f6553-105">**SetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6553-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f6553-106">Attributes and elements</span></span>

<span data-ttu-id="f6553-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f6553-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6553-108">属性</span><span class="sxs-lookup"><span data-stu-id="f6553-108">Attributes</span></span>

<span data-ttu-id="f6553-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f6553-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6553-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f6553-110">Child elements</span></span>

|<span data-ttu-id="f6553-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f6553-111">**Element**</span></span>|<span data-ttu-id="f6553-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6553-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6553-113">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="f6553-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="f6553-114">SetUserOofSettings または GetUserOofSettings の要求をメールボックスのユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="f6553-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
|[<span data-ttu-id="f6553-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="f6553-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="f6553-116">不在の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6553-116">Specifies the OOF settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6553-117">親要素</span><span class="sxs-lookup"><span data-stu-id="f6553-117">Parent elements</span></span>

<span data-ttu-id="f6553-118">なし。</span><span class="sxs-lookup"><span data-stu-id="f6553-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f6553-119">備考</span><span class="sxs-lookup"><span data-stu-id="f6553-119">Remarks</span></span>

<span data-ttu-id="f6553-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="f6553-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="f6553-121">例</span><span class="sxs-lookup"><span data-stu-id="f6553-121">Example</span></span>

<span data-ttu-id="f6553-122">SetUserOofSettings 要求の次の例では、10 日間、不在時の設定を設定します。</span><span class="sxs-lookup"><span data-stu-id="f6553-122">The following example of a SetUserOofSettings request sets an OOF setting for ten days.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="f6553-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="f6553-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6553-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="f6553-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f6553-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f6553-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f6553-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f6553-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f6553-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f6553-127">Validation File</span></span>  <br/> |<span data-ttu-id="f6553-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f6553-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f6553-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f6553-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6553-130">False</span><span class="sxs-lookup"><span data-stu-id="f6553-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6553-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="f6553-131">See also</span></span>



[<span data-ttu-id="f6553-132">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="f6553-132">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

