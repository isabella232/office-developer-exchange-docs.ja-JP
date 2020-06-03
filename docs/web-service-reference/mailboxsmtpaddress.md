---
title: MailboxSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxSmtpAddress
api_type:
- schema
ms.assetid: de7c9035-ebbc-4473-ac14-3b22ce62768c
description: MailboxSmtpAddress 要素は、受信トレイルールを取得または更新するユーザーの SMTP アドレスを表します。または、パスワードの有効期限が切れる日付を取得します。
ms.openlocfilehash: 613e8098210257280bec47f2b22a2d29d04fa07c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530545"
---
# <a name="mailboxsmtpaddress"></a><span data-ttu-id="92e9a-103">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="92e9a-103">MailboxSmtpAddress</span></span>

<span data-ttu-id="92e9a-104">**MailboxSmtpAddress**要素は、受信トレイルールを取得または更新するユーザーの SMTP アドレスを表します。または、パスワードの有効期限が切れる日付を取得します。</span><span class="sxs-lookup"><span data-stu-id="92e9a-104">The **MailboxSmtpAddress** element represents the SMTP address of the user whose Inbox rules are to be retrieved or updated; or whose password expiration date is to be retrieved.</span></span> 
  
```XML
<MailboxSmtpAddress/>
```

<span data-ttu-id="92e9a-105">**string**</span><span class="sxs-lookup"><span data-stu-id="92e9a-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="92e9a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="92e9a-106">Attributes and elements</span></span>

<span data-ttu-id="92e9a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="92e9a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92e9a-108">属性</span><span class="sxs-lookup"><span data-stu-id="92e9a-108">Attributes</span></span>

<span data-ttu-id="92e9a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="92e9a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92e9a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="92e9a-110">Child elements</span></span>

<span data-ttu-id="92e9a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="92e9a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="92e9a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="92e9a-112">Parent elements</span></span>

|<span data-ttu-id="92e9a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="92e9a-113">**Element**</span></span>|<span data-ttu-id="92e9a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="92e9a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92e9a-115">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="92e9a-115">GetInboxRules</span></span>](getinboxrules.md) <br/> |<span data-ttu-id="92e9a-116">サーバーストア内のメールボックスの受信トレイルールを取得するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="92e9a-116">Defines a request to get the Inbox rules on a mailbox in the server store.</span></span>  <br/> |
|[<span data-ttu-id="92e9a-117">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="92e9a-117">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md) <br/> |<span data-ttu-id="92e9a-118">電子メールアカウントのパスワードの有効期限日を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="92e9a-118">Defines a request to get the password expiration date of an email account.</span></span>  <br/> |
|[<span data-ttu-id="92e9a-119">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="92e9a-119">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="92e9a-120">サーバーストア内のメールボックスの受信トレイルールを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="92e9a-120">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="92e9a-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="92e9a-121">Text value</span></span>

<span data-ttu-id="92e9a-122">なし。</span><span class="sxs-lookup"><span data-stu-id="92e9a-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="92e9a-123">注釈</span><span class="sxs-lookup"><span data-stu-id="92e9a-123">Remarks</span></span>

<span data-ttu-id="92e9a-124">**MailboxSmtpAddress**要素は、省略可能な要素です。</span><span class="sxs-lookup"><span data-stu-id="92e9a-124">The **MailboxSmtpAddress** element is an optional element.</span></span> <span data-ttu-id="92e9a-125">**MailboxSmtpAddress**要素を省略すると、ログオンしているユーザーのアドレスが使用されます。</span><span class="sxs-lookup"><span data-stu-id="92e9a-125">If the **MailboxSmtpAddress** element is omitted, the address of the logged on user is used.</span></span> 
  
<span data-ttu-id="92e9a-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="92e9a-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92e9a-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="92e9a-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92e9a-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="92e9a-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92e9a-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="92e9a-129">Schema Name</span></span>  <br/> |<span data-ttu-id="92e9a-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="92e9a-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="92e9a-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="92e9a-131">Validation File</span></span>  <br/> |<span data-ttu-id="92e9a-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="92e9a-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92e9a-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="92e9a-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="92e9a-134">正しい</span><span class="sxs-lookup"><span data-stu-id="92e9a-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92e9a-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="92e9a-135">See also</span></span>

- [<span data-ttu-id="92e9a-136">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="92e9a-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)
- [<span data-ttu-id="92e9a-137">GetPasswordExpirationDate 操作</span><span class="sxs-lookup"><span data-stu-id="92e9a-137">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="92e9a-138">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="92e9a-138">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="92e9a-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="92e9a-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

