---
title: ForwardAsAttachmentToRecipients 添付ファイル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ForwardAsAttachmentToRecipients
api_type:
- schema
ms.assetid: 8649ea14-672f-43c9-b10a-a2b02efd5867
description: Forwardasattachmenttorattachmentpiattachment要素は、メッセージが添付ファイルとして転送される電子メールアドレスを示します。
ms.openlocfilehash: bf8c3563460eea811602074bf16f9253b4610832
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44453337"
---
# <a name="forwardasattachmenttorecipients"></a><span data-ttu-id="69f9d-103">ForwardAsAttachmentToRecipients 添付ファイル</span><span class="sxs-lookup"><span data-stu-id="69f9d-103">ForwardAsAttachmentToRecipients</span></span>

<span data-ttu-id="69f9d-104">**Forwardasattachmenttorattachmentpiattachment要素**は、メッセージが添付ファイルとして転送される電子メールアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="69f9d-104">The **ForwardAsAttachmentToRecipients** element indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span> 
  
```XML
<ForwardAsAttachmentToRecipients>
   <Address/>
</ForwardAsAttachmentToRecipients>
```

 <span data-ttu-id="69f9d-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="69f9d-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69f9d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="69f9d-106">Attributes and elements</span></span>

<span data-ttu-id="69f9d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="69f9d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69f9d-108">属性</span><span class="sxs-lookup"><span data-stu-id="69f9d-108">Attributes</span></span>

<span data-ttu-id="69f9d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="69f9d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69f9d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="69f9d-110">Child elements</span></span>

|<span data-ttu-id="69f9d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="69f9d-111">**Element**</span></span>|<span data-ttu-id="69f9d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="69f9d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69f9d-113">Address (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="69f9d-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="69f9d-114">完全に解決された電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="69f9d-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69f9d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="69f9d-115">Parent elements</span></span>

|<span data-ttu-id="69f9d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="69f9d-116">**Element**</span></span>|<span data-ttu-id="69f9d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="69f9d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69f9d-118">Actions</span><span class="sxs-lookup"><span data-stu-id="69f9d-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="69f9d-119">条件が満たされたときに、メッセージに対して実行できるアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="69f9d-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="69f9d-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="69f9d-120">Text value</span></span>

<span data-ttu-id="69f9d-121">なし。</span><span class="sxs-lookup"><span data-stu-id="69f9d-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="69f9d-122">注釈</span><span class="sxs-lookup"><span data-stu-id="69f9d-122">Remarks</span></span>

<span data-ttu-id="69f9d-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="69f9d-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69f9d-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="69f9d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69f9d-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="69f9d-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="69f9d-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="69f9d-126">Schema Name</span></span>  <br/> |<span data-ttu-id="69f9d-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="69f9d-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="69f9d-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="69f9d-128">Validation File</span></span>  <br/> |<span data-ttu-id="69f9d-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="69f9d-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="69f9d-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="69f9d-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="69f9d-131">正しい</span><span class="sxs-lookup"><span data-stu-id="69f9d-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69f9d-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="69f9d-132">See also</span></span>



- [<span data-ttu-id="69f9d-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="69f9d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

