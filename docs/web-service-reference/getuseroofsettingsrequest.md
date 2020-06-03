---
title: GetUserOofSettingsRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettingsRequest
api_type:
- schema
ms.assetid: 15dea99c-7f5d-4af1-82ff-4255127fe567
description: GetUserOofSettingsRequest 要素は、メールボックスユーザーの不在時 (OOF) の設定を取得するために使用される引数を含むルート要素です。
ms.openlocfilehash: f515e8cf016d3aff6c652ae92a0da71a8f0a5f6b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457831"
---
# <a name="getuseroofsettingsrequest"></a><span data-ttu-id="02b53-103">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="02b53-103">GetUserOofSettingsRequest</span></span>

<span data-ttu-id="02b53-104">**Getuseroofsettingsrequest**要素は、メールボックスユーザーの不在時 (OOF) の設定を取得するために使用される引数を含むルート要素です。</span><span class="sxs-lookup"><span data-stu-id="02b53-104">The **GetUserOofSettingsRequest** element is the root element that contains the arguments used to get a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<GetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
</GetUserOofSettingsRequest>
```

 <span data-ttu-id="02b53-105">**GetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="02b53-105">**GetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02b53-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="02b53-106">Attributes and elements</span></span>

<span data-ttu-id="02b53-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="02b53-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02b53-108">属性</span><span class="sxs-lookup"><span data-stu-id="02b53-108">Attributes</span></span>

<span data-ttu-id="02b53-109">なし。</span><span class="sxs-lookup"><span data-stu-id="02b53-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02b53-110">子要素</span><span class="sxs-lookup"><span data-stu-id="02b53-110">Child elements</span></span>

|<span data-ttu-id="02b53-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="02b53-111">**Element**</span></span>|<span data-ttu-id="02b53-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="02b53-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02b53-113">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="02b53-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="02b53-114">SetUserOofSettings または GetUserOofSettings 要求のメールボックスユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="02b53-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="02b53-115">親要素</span><span class="sxs-lookup"><span data-stu-id="02b53-115">Parent elements</span></span>

<span data-ttu-id="02b53-116">なし。</span><span class="sxs-lookup"><span data-stu-id="02b53-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="02b53-117">注釈</span><span class="sxs-lookup"><span data-stu-id="02b53-117">Remarks</span></span>

<span data-ttu-id="02b53-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="02b53-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="02b53-119">例</span><span class="sxs-lookup"><span data-stu-id="02b53-119">Example</span></span>

<span data-ttu-id="02b53-120">1人のユーザーの OOF 情報を取得する、GetUserOofSettings 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="02b53-120">The following is an example of a GetUserOofSettings request that gets a single user's OOF information.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="02b53-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="02b53-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02b53-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="02b53-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="02b53-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="02b53-123">Schema Name</span></span>  <br/> |<span data-ttu-id="02b53-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="02b53-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="02b53-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="02b53-125">Validation File</span></span>  <br/> |<span data-ttu-id="02b53-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="02b53-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="02b53-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="02b53-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="02b53-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="02b53-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02b53-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="02b53-129">See also</span></span>



[<span data-ttu-id="02b53-130">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="02b53-130">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)

