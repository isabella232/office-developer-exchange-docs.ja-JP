---
title: AllowExternalOof
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowExternalOof
api_type:
- schema
ms.assetid: e5387172-5b92-4bb1-8394-180e9c7ff771
description: AllowExternalOof 要素には、外部の不在時 (OOF) メッセージが送信されるユーザーを識別する値が含まれています。
ms.openlocfilehash: e4934bc4bc86e1f9f764279a13ecaeca073d9e5d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464813"
---
# <a name="allowexternaloof"></a><span data-ttu-id="23967-103">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="23967-103">AllowExternalOof</span></span>

<span data-ttu-id="23967-104">**AllowExternalOof**要素には、外部の不在時 (OOF) メッセージが送信されるユーザーを識別する値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="23967-104">The **AllowExternalOof** element contains a value that identifies to whom external Out of Office (OOF) messages are sent.</span></span> 
  
- [<span data-ttu-id="23967-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="23967-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
- [<span data-ttu-id="23967-106">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="23967-106">AllowExternalOof</span></span>](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 <span data-ttu-id="23967-107">**ExternalAudience**</span><span class="sxs-lookup"><span data-stu-id="23967-107">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23967-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="23967-108">Attributes and elements</span></span>

<span data-ttu-id="23967-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="23967-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23967-110">属性</span><span class="sxs-lookup"><span data-stu-id="23967-110">Attributes</span></span>

<span data-ttu-id="23967-111">なし。</span><span class="sxs-lookup"><span data-stu-id="23967-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23967-112">子要素</span><span class="sxs-lookup"><span data-stu-id="23967-112">Child elements</span></span>

<span data-ttu-id="23967-113">なし。</span><span class="sxs-lookup"><span data-stu-id="23967-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="23967-114">親要素</span><span class="sxs-lookup"><span data-stu-id="23967-114">Parent elements</span></span>

|<span data-ttu-id="23967-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="23967-115">**Element**</span></span>|<span data-ttu-id="23967-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="23967-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23967-117">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="23967-117">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="23967-118">応答結果とユーザーの OOF 設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="23967-118">Contains the response results and the OOF settings for a user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="23967-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="23967-119">Text value</span></span>

<span data-ttu-id="23967-120">この要素にはテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="23967-120">A text value is required for this element.</span></span> <span data-ttu-id="23967-121">次の表に、この要素で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="23967-121">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="23967-122">**値**</span><span class="sxs-lookup"><span data-stu-id="23967-122">**Value**</span></span>|<span data-ttu-id="23967-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="23967-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="23967-124">**なし**</span><span class="sxs-lookup"><span data-stu-id="23967-124">**None**</span></span> <br/> |<span data-ttu-id="23967-125">メールボックスユーザーの組織外の電子メール送信者は、ユーザーにメッセージを送信すると、外部の不在時メッセージ応答を受信しません。</span><span class="sxs-lookup"><span data-stu-id="23967-125">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="23967-126">**一般的**</span><span class="sxs-lookup"><span data-stu-id="23967-126">**Known**</span></span> <br/> |<span data-ttu-id="23967-127">メールボックスユーザーの組織外の電子メール送信者がユーザーにメッセージを送信すると、送信者がユーザーの Exchange ストアの連絡先リストにある場合にのみ、外部の OOF メッセージ応答が受信されます。</span><span class="sxs-lookup"><span data-stu-id="23967-127">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="23967-128">**All**</span><span class="sxs-lookup"><span data-stu-id="23967-128">**All**</span></span> <br/> |<span data-ttu-id="23967-129">メールボックスユーザーの組織外の電子メール送信者は、ユーザーにメッセージを送信すると、外部の OOF メッセージ応答を受信します。</span><span class="sxs-lookup"><span data-stu-id="23967-129">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="23967-130">注釈</span><span class="sxs-lookup"><span data-stu-id="23967-130">Remarks</span></span>

<span data-ttu-id="23967-131">この要素は、 [Externalaudience](externalaudience.md)要素と同じ型を共有します。</span><span class="sxs-lookup"><span data-stu-id="23967-131">This element shares the same type as the [ExternalAudience](externalaudience.md) element.</span></span> 
  
<span data-ttu-id="23967-132">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="23967-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23967-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="23967-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23967-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="23967-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="23967-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="23967-135">Schema Name</span></span>  <br/> |<span data-ttu-id="23967-136">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="23967-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="23967-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="23967-137">Validation File</span></span>  <br/> |<span data-ttu-id="23967-138">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="23967-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="23967-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="23967-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="23967-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="23967-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="23967-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="23967-141">See also</span></span>

- [<span data-ttu-id="23967-142">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="23967-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md) 
- [<span data-ttu-id="23967-143">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="23967-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

