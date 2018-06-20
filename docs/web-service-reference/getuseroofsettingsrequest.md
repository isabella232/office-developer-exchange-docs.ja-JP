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
description: GetUserOofSettingsRequest 要素は、メールボックスにユーザーの Office (OOF) の設定を取得するための引数を含むルート要素です。
ms.openlocfilehash: e64818961283f90e447e2044cf7f918eccd21f06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831692"
---
# <a name="getuseroofsettingsrequest"></a><span data-ttu-id="8a6f1-103">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="8a6f1-103">GetUserOofSettingsRequest</span></span>

<span data-ttu-id="8a6f1-104">**GetUserOofSettingsRequest**要素は、メールボックスにユーザーの Office (OOF) の設定を取得するための引数を含むルート要素です。</span><span class="sxs-lookup"><span data-stu-id="8a6f1-104">The **GetUserOofSettingsRequest** element is the root element that contains the arguments used to get a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<GetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
</GetUserOofSettingsRequest>
```

 <span data-ttu-id="8a6f1-105">**GetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="8a6f1-105">**GetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a6f1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8a6f1-106">Attributes and elements</span></span>

<span data-ttu-id="8a6f1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8a6f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a6f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="8a6f1-108">Attributes</span></span>

<span data-ttu-id="8a6f1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8a6f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a6f1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8a6f1-110">Child elements</span></span>

|<span data-ttu-id="8a6f1-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="8a6f1-111">**Element**</span></span>|<span data-ttu-id="8a6f1-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8a6f1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a6f1-113">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="8a6f1-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="8a6f1-114">SetUserOofSettings または GetUserOofSettings の要求をメールボックスのユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="8a6f1-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8a6f1-115">親要素</span><span class="sxs-lookup"><span data-stu-id="8a6f1-115">Parent elements</span></span>

<span data-ttu-id="8a6f1-116">なし。</span><span class="sxs-lookup"><span data-stu-id="8a6f1-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8a6f1-117">備考</span><span class="sxs-lookup"><span data-stu-id="8a6f1-117">Remarks</span></span>

<span data-ttu-id="8a6f1-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="8a6f1-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="8a6f1-119">例</span><span class="sxs-lookup"><span data-stu-id="8a6f1-119">Example</span></span>

<span data-ttu-id="8a6f1-120">次に、単一のユーザーの不在時の情報を取得する GetUserOofSettings 要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="8a6f1-120">The following is an example of a GetUserOofSettings request that gets a single user's OOF information.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="8a6f1-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="8a6f1-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a6f1-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="8a6f1-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8a6f1-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8a6f1-123">Schema Name</span></span>  <br/> |<span data-ttu-id="8a6f1-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="8a6f1-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8a6f1-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8a6f1-125">Validation File</span></span>  <br/> |<span data-ttu-id="8a6f1-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8a6f1-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8a6f1-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8a6f1-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a6f1-128">False</span><span class="sxs-lookup"><span data-stu-id="8a6f1-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a6f1-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="8a6f1-129">See also</span></span>



[<span data-ttu-id="8a6f1-130">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="8a6f1-130">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)

