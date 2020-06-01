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
description: SetUserOofSettingsRequest 要素には、メールボックスユーザーの不在時 (OOF) の設定を設定するために使用する引数が含まれています。
ms.openlocfilehash: 10edc9809fd72f80c316de1c6688eaedec4f93df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466151"
---
# <a name="setuseroofsettingsrequest"></a><span data-ttu-id="0a851-103">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="0a851-103">SetUserOofSettingsRequest</span></span>

<span data-ttu-id="0a851-104">**Setuseroofsettingsrequest**要素には、メールボックスユーザーの不在時 (OOF) の設定を設定するために使用する引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0a851-104">The **SetUserOofSettingsRequest** element contains the arguments used to set a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<SetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
   <UserOofSettings>...</UserOofSettings>
<SetUserOofSettingsRequest>
```

 <span data-ttu-id="0a851-105">**SetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="0a851-105">**SetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a851-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0a851-106">Attributes and elements</span></span>

<span data-ttu-id="0a851-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0a851-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a851-108">属性</span><span class="sxs-lookup"><span data-stu-id="0a851-108">Attributes</span></span>

<span data-ttu-id="0a851-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0a851-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a851-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0a851-110">Child elements</span></span>

|<span data-ttu-id="0a851-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="0a851-111">**Element**</span></span>|<span data-ttu-id="0a851-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0a851-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a851-113">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="0a851-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="0a851-114">SetUserOofSettings または GetUserOofSettings 要求のメールボックスユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="0a851-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
|[<span data-ttu-id="0a851-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="0a851-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="0a851-116">OOF 設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a851-116">Specifies the OOF settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0a851-117">親要素</span><span class="sxs-lookup"><span data-stu-id="0a851-117">Parent elements</span></span>

<span data-ttu-id="0a851-118">なし。</span><span class="sxs-lookup"><span data-stu-id="0a851-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0a851-119">注釈</span><span class="sxs-lookup"><span data-stu-id="0a851-119">Remarks</span></span>

<span data-ttu-id="0a851-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0a851-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="0a851-121">例</span><span class="sxs-lookup"><span data-stu-id="0a851-121">Example</span></span>

<span data-ttu-id="0a851-122">SetUserOofSettings 要求の次の例では、OOF 設定を10日間設定しています。</span><span class="sxs-lookup"><span data-stu-id="0a851-122">The following example of a SetUserOofSettings request sets an OOF setting for ten days.</span></span>
  
```xml
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

## <a name="element-information"></a><span data-ttu-id="0a851-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0a851-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a851-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="0a851-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0a851-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0a851-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0a851-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0a851-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0a851-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0a851-127">Validation File</span></span>  <br/> |<span data-ttu-id="0a851-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0a851-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0a851-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0a851-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="0a851-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="0a851-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a851-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="0a851-131">See also</span></span>



[<span data-ttu-id="0a851-132">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="0a851-132">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

