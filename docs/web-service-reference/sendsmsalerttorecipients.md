---
title: SendSMSAlertToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendSMSAlertToRecipients
api_type:
- schema
ms.assetid: c4dd000b-11b6-4b7b-91e0-dbfeae11d770
description: SendSMSAlertToRecipients 要素は、短いメッセージサービス (SMS) の通知が送信される携帯電話の番号を示します。
ms.openlocfilehash: ed17bf9ad20a51cbead4b86f385a53d19562fa64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464848"
---
# <a name="sendsmsalerttorecipients"></a><span data-ttu-id="acc5c-103">SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="acc5c-103">SendSMSAlertToRecipients</span></span>

<span data-ttu-id="acc5c-104">**SendSMSAlertToRecipients**要素は、短いメッセージサービス (SMS) の通知が送信される携帯電話の番号を示します。</span><span class="sxs-lookup"><span data-stu-id="acc5c-104">The **SendSMSAlertToRecipients** element indicates the mobile phone numbers to which a Short Message Service (SMS) alert is to be sent.</span></span> 
  
```XML
<SendSMSAlertToRecipients>
   <Address/>
</SendSMSAlertToRecipients>
```

 <span data-ttu-id="acc5c-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="acc5c-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="acc5c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="acc5c-106">Attributes and elements</span></span>

<span data-ttu-id="acc5c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="acc5c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="acc5c-108">属性</span><span class="sxs-lookup"><span data-stu-id="acc5c-108">Attributes</span></span>

<span data-ttu-id="acc5c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="acc5c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="acc5c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="acc5c-110">Child elements</span></span>

|<span data-ttu-id="acc5c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="acc5c-111">**Element**</span></span>|<span data-ttu-id="acc5c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="acc5c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="acc5c-113">Address (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="acc5c-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="acc5c-114">完全に解決された電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="acc5c-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="acc5c-115">親要素</span><span class="sxs-lookup"><span data-stu-id="acc5c-115">Parent elements</span></span>

|<span data-ttu-id="acc5c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="acc5c-116">**Element**</span></span>|<span data-ttu-id="acc5c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="acc5c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="acc5c-118">Actions</span><span class="sxs-lookup"><span data-stu-id="acc5c-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="acc5c-119">条件が満たされたときに、メッセージに対して実行できるアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="acc5c-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="acc5c-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="acc5c-120">Text value</span></span>

<span data-ttu-id="acc5c-121">なし。</span><span class="sxs-lookup"><span data-stu-id="acc5c-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="acc5c-122">注釈</span><span class="sxs-lookup"><span data-stu-id="acc5c-122">Remarks</span></span>

<span data-ttu-id="acc5c-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="acc5c-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="acc5c-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="acc5c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="acc5c-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="acc5c-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="acc5c-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="acc5c-126">Schema Name</span></span>  <br/> |<span data-ttu-id="acc5c-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="acc5c-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="acc5c-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="acc5c-128">Validation File</span></span>  <br/> |<span data-ttu-id="acc5c-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="acc5c-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="acc5c-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="acc5c-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="acc5c-131">正しい</span><span class="sxs-lookup"><span data-stu-id="acc5c-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="acc5c-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="acc5c-132">See also</span></span>



- [<span data-ttu-id="acc5c-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="acc5c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

