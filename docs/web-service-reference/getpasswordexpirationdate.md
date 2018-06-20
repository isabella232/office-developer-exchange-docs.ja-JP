---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: GetPasswordExpirationDate 要素は、電子メール アカウントのパスワードの有効期限の日付を取得する要求を定義します。 この要素は、GetPasswordExpirationDate 操作の操作の基本要素です。
ms.openlocfilehash: a9e0955566372f7b99c48c56e62ce2c5025f9f95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760819"
---
# <a name="getpasswordexpirationdate"></a><span data-ttu-id="fe02b-104">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="fe02b-104">GetPasswordExpirationDate</span></span>

<span data-ttu-id="fe02b-105">**GetPasswordExpirationDate**要素は、電子メール アカウントのパスワードの有効期限の日付を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="fe02b-105">The **GetPasswordExpirationDate** element defines a request to get the password expiration date for an email account.</span></span> <span data-ttu-id="fe02b-106">この要素は、 [GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)の操作の基本要素です。</span><span class="sxs-lookup"><span data-stu-id="fe02b-106">This element is the base element for the [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation.</span></span> 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 <span data-ttu-id="fe02b-107">**GetPasswordExpirationDateType**</span><span class="sxs-lookup"><span data-stu-id="fe02b-107">**GetPasswordExpirationDateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fe02b-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fe02b-108">Attributes and elements</span></span>

<span data-ttu-id="fe02b-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fe02b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe02b-110">属性</span><span class="sxs-lookup"><span data-stu-id="fe02b-110">Attributes</span></span>

<span data-ttu-id="fe02b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fe02b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fe02b-112">子要素</span><span class="sxs-lookup"><span data-stu-id="fe02b-112">Child elements</span></span>

|<span data-ttu-id="fe02b-113">**要素名**</span><span class="sxs-lookup"><span data-stu-id="fe02b-113">**Element name**</span></span>|<span data-ttu-id="fe02b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="fe02b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe02b-115">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="fe02b-115">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="fe02b-116">パスワード有効期限の日付が返される対象の電子メール アカウントの電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="fe02b-116">Represents the email address of the email account for which the password expiration date is to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fe02b-117">親要素</span><span class="sxs-lookup"><span data-stu-id="fe02b-117">Parent elements</span></span>

<span data-ttu-id="fe02b-118">なし。</span><span class="sxs-lookup"><span data-stu-id="fe02b-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fe02b-119">備考</span><span class="sxs-lookup"><span data-stu-id="fe02b-119">Remarks</span></span>

<span data-ttu-id="fe02b-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fe02b-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="fe02b-121">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fe02b-121">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe02b-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="fe02b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe02b-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="fe02b-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fe02b-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fe02b-124">Schema Name</span></span>  <br/> |<span data-ttu-id="fe02b-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="fe02b-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fe02b-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fe02b-126">Validation File</span></span>  <br/> |<span data-ttu-id="fe02b-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fe02b-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fe02b-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fe02b-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="fe02b-129">False</span><span class="sxs-lookup"><span data-stu-id="fe02b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fe02b-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="fe02b-130">See also</span></span>



[<span data-ttu-id="fe02b-131">GetPasswordExpirationDate 操作</span><span class="sxs-lookup"><span data-stu-id="fe02b-131">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)


- [<span data-ttu-id="fe02b-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fe02b-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

