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
description: SendSMSAlertToRecipients 要素では、ショート メッセージ サービス (SMS) アラートが送信するのには携帯電話の番号を示します。
ms.openlocfilehash: b28202c71257fccca67879713d5d7df03f69b06d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833347"
---
# <a name="sendsmsalerttorecipients"></a><span data-ttu-id="912aa-103">SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="912aa-103">SendSMSAlertToRecipients</span></span>

<span data-ttu-id="912aa-104">**SendSMSAlertToRecipients**要素では、ショート メッセージ サービス (SMS) アラートが送信するのには携帯電話の番号を示します。</span><span class="sxs-lookup"><span data-stu-id="912aa-104">The **SendSMSAlertToRecipients** element indicates the mobile phone numbers to which a Short Message Service (SMS) alert is to be sent.</span></span> 
  
```XML
<SendSMSAlertToRecipients>
   <Address/>
</SendSMSAlertToRecipients>
```

 <span data-ttu-id="912aa-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="912aa-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="912aa-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="912aa-106">Attributes and elements</span></span>

<span data-ttu-id="912aa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="912aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="912aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="912aa-108">Attributes</span></span>

<span data-ttu-id="912aa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="912aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="912aa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="912aa-110">Child elements</span></span>

|<span data-ttu-id="912aa-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="912aa-111">**Element**</span></span>|<span data-ttu-id="912aa-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="912aa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="912aa-113">アドレス (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="912aa-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="912aa-114">完全に解決された電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="912aa-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="912aa-115">親要素</span><span class="sxs-lookup"><span data-stu-id="912aa-115">Parent elements</span></span>

|<span data-ttu-id="912aa-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="912aa-116">**Element**</span></span>|<span data-ttu-id="912aa-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="912aa-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="912aa-118">アクション</span><span class="sxs-lookup"><span data-stu-id="912aa-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="912aa-119">条件が満たされるときに、メッセージに対して実行される使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="912aa-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="912aa-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="912aa-120">Text value</span></span>

<span data-ttu-id="912aa-121">なし。</span><span class="sxs-lookup"><span data-stu-id="912aa-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="912aa-122">備考</span><span class="sxs-lookup"><span data-stu-id="912aa-122">Remarks</span></span>

<span data-ttu-id="912aa-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="912aa-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="912aa-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="912aa-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="912aa-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="912aa-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="912aa-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="912aa-126">Schema Name</span></span>  <br/> |<span data-ttu-id="912aa-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="912aa-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="912aa-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="912aa-128">Validation File</span></span>  <br/> |<span data-ttu-id="912aa-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="912aa-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="912aa-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="912aa-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="912aa-131">True</span><span class="sxs-lookup"><span data-stu-id="912aa-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="912aa-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="912aa-132">See also</span></span>



- [<span data-ttu-id="912aa-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="912aa-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

