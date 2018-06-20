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
description: AllowExternalOof 要素には、外部の Office (OOF) メッセージを送信するを識別する値が含まれています。
ms.openlocfilehash: 1c87a51676bf6e44b2e650a4e973d0ab89a52e31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759316"
---
# <a name="allowexternaloof"></a><span data-ttu-id="6deed-103">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="6deed-103">AllowExternalOof</span></span>

<span data-ttu-id="6deed-104">**AllowExternalOof**要素には、外部の Office (OOF) メッセージを送信するを識別する値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6deed-104">The **AllowExternalOof** element contains a value that identifies to whom external Out of Office (OOF) messages are sent.</span></span> 
  
- [<span data-ttu-id="6deed-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="6deed-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
- [<span data-ttu-id="6deed-106">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="6deed-106">AllowExternalOof</span></span>](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 <span data-ttu-id="6deed-107">**ExternalAudience**</span><span class="sxs-lookup"><span data-stu-id="6deed-107">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6deed-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6deed-108">Attributes and elements</span></span>

<span data-ttu-id="6deed-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6deed-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6deed-110">属性</span><span class="sxs-lookup"><span data-stu-id="6deed-110">Attributes</span></span>

<span data-ttu-id="6deed-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6deed-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6deed-112">子要素</span><span class="sxs-lookup"><span data-stu-id="6deed-112">Child elements</span></span>

<span data-ttu-id="6deed-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6deed-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6deed-114">親要素</span><span class="sxs-lookup"><span data-stu-id="6deed-114">Parent elements</span></span>

|<span data-ttu-id="6deed-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="6deed-115">**Element**</span></span>|<span data-ttu-id="6deed-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="6deed-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6deed-117">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="6deed-117">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="6deed-118">応答結果とユーザーの不在時の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6deed-118">Contains the response results and the OOF settings for a user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6deed-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6deed-119">Text value</span></span>

<span data-ttu-id="6deed-120">テキスト値は、この要素の必要があります。</span><span class="sxs-lookup"><span data-stu-id="6deed-120">A text value is required for this element.</span></span> <span data-ttu-id="6deed-121">次の表は、この要素の有効な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="6deed-121">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="6deed-122">**値**</span><span class="sxs-lookup"><span data-stu-id="6deed-122">**Value**</span></span>|<span data-ttu-id="6deed-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="6deed-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6deed-124">**None**</span><span class="sxs-lookup"><span data-stu-id="6deed-124">**None**</span></span> <br/> |<span data-ttu-id="6deed-125">メールボックス ユーザーの組織外のユーザーにメッセージを送信するメールの送信者は、外部の OOF メッセージの応答を受信しません。</span><span class="sxs-lookup"><span data-stu-id="6deed-125">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="6deed-126">**呼ばれる**</span><span class="sxs-lookup"><span data-stu-id="6deed-126">**Known**</span></span> <br/> |<span data-ttu-id="6deed-127">メールボックス ユーザーの組織の外部ユーザーへのメッセージのみが表示されます、外部の OOF メッセージ応答送信者がユーザーの Exchange の場合に送信したメールの送信者は、連絡先リストを保存します。</span><span class="sxs-lookup"><span data-stu-id="6deed-127">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="6deed-128">**All**</span><span class="sxs-lookup"><span data-stu-id="6deed-128">**All**</span></span> <br/> |<span data-ttu-id="6deed-129">メールボックス ユーザーの組織外のユーザーにメッセージを送信するメールの送信者が外部の OOF メッセージの応答を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="6deed-129">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6deed-130">備考</span><span class="sxs-lookup"><span data-stu-id="6deed-130">Remarks</span></span>

<span data-ttu-id="6deed-131">この要素は、 [ExternalAudience](externalaudience.md)要素と同じ型を共有します。</span><span class="sxs-lookup"><span data-stu-id="6deed-131">This element shares the same type as the [ExternalAudience](externalaudience.md) element.</span></span> 
  
<span data-ttu-id="6deed-132">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="6deed-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6deed-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="6deed-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6deed-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="6deed-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6deed-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6deed-135">Schema Name</span></span>  <br/> |<span data-ttu-id="6deed-136">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6deed-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6deed-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6deed-137">Validation File</span></span>  <br/> |<span data-ttu-id="6deed-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6deed-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6deed-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6deed-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="6deed-140">False</span><span class="sxs-lookup"><span data-stu-id="6deed-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6deed-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="6deed-141">See also</span></span>

- [<span data-ttu-id="6deed-142">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="6deed-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md) 
- [<span data-ttu-id="6deed-143">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="6deed-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

