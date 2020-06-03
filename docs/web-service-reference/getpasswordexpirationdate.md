---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: GetPasswordExpirationDate 要素は、電子メールアカウントのパスワードの有効期限日を取得する要求を定義します。 この要素は、GetPasswordExpirationDate 操作操作の基本要素です。
ms.openlocfilehash: ececbf51f71c7d87705d727229fce2314d922efb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456494"
---
# <a name="getpasswordexpirationdate"></a><span data-ttu-id="64ffe-104">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="64ffe-104">GetPasswordExpirationDate</span></span>

<span data-ttu-id="64ffe-105">**GetPasswordExpirationDate**要素は、電子メールアカウントのパスワードの有効期限日を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="64ffe-105">The **GetPasswordExpirationDate** element defines a request to get the password expiration date for an email account.</span></span> <span data-ttu-id="64ffe-106">この要素は、 [GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)操作の基本要素です。</span><span class="sxs-lookup"><span data-stu-id="64ffe-106">This element is the base element for the [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation.</span></span> 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 <span data-ttu-id="64ffe-107">**GetPasswordExpirationDateType**</span><span class="sxs-lookup"><span data-stu-id="64ffe-107">**GetPasswordExpirationDateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64ffe-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="64ffe-108">Attributes and elements</span></span>

<span data-ttu-id="64ffe-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="64ffe-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64ffe-110">属性</span><span class="sxs-lookup"><span data-stu-id="64ffe-110">Attributes</span></span>

<span data-ttu-id="64ffe-111">なし。</span><span class="sxs-lookup"><span data-stu-id="64ffe-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64ffe-112">子要素</span><span class="sxs-lookup"><span data-stu-id="64ffe-112">Child elements</span></span>

|<span data-ttu-id="64ffe-113">**要素名**</span><span class="sxs-lookup"><span data-stu-id="64ffe-113">**Element name**</span></span>|<span data-ttu-id="64ffe-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="64ffe-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64ffe-115">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="64ffe-115">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="64ffe-116">パスワードの有効期限の日付を返す電子メールアカウントの電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="64ffe-116">Represents the email address of the email account for which the password expiration date is to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="64ffe-117">親要素</span><span class="sxs-lookup"><span data-stu-id="64ffe-117">Parent elements</span></span>

<span data-ttu-id="64ffe-118">なし。</span><span class="sxs-lookup"><span data-stu-id="64ffe-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="64ffe-119">注釈</span><span class="sxs-lookup"><span data-stu-id="64ffe-119">Remarks</span></span>

<span data-ttu-id="64ffe-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="64ffe-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="64ffe-121">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="64ffe-121">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64ffe-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="64ffe-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64ffe-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="64ffe-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="64ffe-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="64ffe-124">Schema Name</span></span>  <br/> |<span data-ttu-id="64ffe-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="64ffe-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="64ffe-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="64ffe-126">Validation File</span></span>  <br/> |<span data-ttu-id="64ffe-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="64ffe-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="64ffe-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="64ffe-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="64ffe-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="64ffe-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64ffe-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="64ffe-130">See also</span></span>



[<span data-ttu-id="64ffe-131">GetPasswordExpirationDate 操作</span><span class="sxs-lookup"><span data-stu-id="64ffe-131">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)


- [<span data-ttu-id="64ffe-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="64ffe-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

