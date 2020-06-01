---
title: 不在
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutOfOffice
api_type:
- schema
ms.assetid: fe1256ab-5c0f-467d-abb3-b38a2dc312ae
description: 不在要素は、応答メッセージと、応答メッセージを送信するまでの時間を表します。
ms.openlocfilehash: 082a81b62e2b783b302b3e749e0066131a46d73e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456900"
---
# <a name="outofoffice"></a><span data-ttu-id="1dfac-103">不在</span><span class="sxs-lookup"><span data-stu-id="1dfac-103">OutOfOffice</span></span>

<span data-ttu-id="1dfac-104">**不在**要素は、応答メッセージと、応答メッセージを送信するまでの時間を表します。</span><span class="sxs-lookup"><span data-stu-id="1dfac-104">The **OutOfOffice** element represents the response message and a duration time for sending the response message.</span></span> 
  
```XML
<OutOfOffice>
   <ReplyBody/>
   <Duration/>
</OutOfOffice>
```

```XML
<OutOfOffice>
   <ReplyBody/>
</OutOfOffice>
```

<span data-ttu-id="1dfac-105">**OutOfOfficeMailTip**</span><span class="sxs-lookup"><span data-stu-id="1dfac-105">**OutOfOfficeMailTip**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1dfac-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1dfac-106">Attributes and elements</span></span>

<span data-ttu-id="1dfac-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1dfac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1dfac-108">属性</span><span class="sxs-lookup"><span data-stu-id="1dfac-108">Attributes</span></span>

<span data-ttu-id="1dfac-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1dfac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1dfac-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1dfac-110">Child elements</span></span>

|<span data-ttu-id="1dfac-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1dfac-111">**Element**</span></span>|<span data-ttu-id="1dfac-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1dfac-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dfac-113">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="1dfac-113">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="1dfac-114">不在 (OOF) メッセージと、メッセージに使用する言語が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1dfac-114">Contains an Out of Office (OOF) message and the language used for the message.</span></span>  <br/> |
|[<span data-ttu-id="1dfac-115">Duration (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="1dfac-115">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="1dfac-116">[Oofstate](oofstate.md)要素が [スケジュール済み] に設定されている場合に、不在時の状態が有効になる期間を含みます。</span><span class="sxs-lookup"><span data-stu-id="1dfac-116">Contains the duration that the OOF status is enabled if the [OofState](oofstate.md) element is set to Scheduled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1dfac-117">親要素</span><span class="sxs-lookup"><span data-stu-id="1dfac-117">Parent elements</span></span>

|<span data-ttu-id="1dfac-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="1dfac-118">**Element**</span></span>|<span data-ttu-id="1dfac-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="1dfac-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dfac-120">メールヒント</span><span class="sxs-lookup"><span data-stu-id="1dfac-120">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="1dfac-121">さまざまな種類のメールヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="1dfac-121">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1dfac-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1dfac-122">Text value</span></span>

<span data-ttu-id="1dfac-123">なし。</span><span class="sxs-lookup"><span data-stu-id="1dfac-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1dfac-124">注釈</span><span class="sxs-lookup"><span data-stu-id="1dfac-124">Remarks</span></span>

<span data-ttu-id="1dfac-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1dfac-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1dfac-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1dfac-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1dfac-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="1dfac-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1dfac-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1dfac-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1dfac-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1dfac-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="1dfac-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1dfac-130">Validation File</span></span>  <br/> |<span data-ttu-id="1dfac-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1dfac-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1dfac-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1dfac-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="1dfac-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="1dfac-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1dfac-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="1dfac-134">See also</span></span>

- [<span data-ttu-id="1dfac-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1dfac-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

