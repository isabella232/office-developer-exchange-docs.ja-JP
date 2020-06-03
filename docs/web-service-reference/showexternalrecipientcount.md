---
title: Showexternal受信者カウント
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: Showexternalrecipients Count 要素は、GetMailTips ヒント操作のコンシューマーが、メッセージの宛先である外部受信者の数を示すメールヒントを表示する必要があるかどうかを示します。
ms.openlocfilehash: fc32e5c4a95f0e33b5532af9c77d31bd6446e641
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460471"
---
# <a name="showexternalrecipientcount"></a><span data-ttu-id="a38e4-103">Showexternal受信者カウント</span><span class="sxs-lookup"><span data-stu-id="a38e4-103">ShowExternalRecipientCount</span></span>

<span data-ttu-id="a38e4-104">**Showexternalrecipients count**要素は、 [getmailtips ヒント操作](getmailtips-operation.md)のコンシューマーが、メッセージの宛先である外部受信者の数を示すメールヒントを表示する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a38e4-104">The **ShowExternalRecipientCount** element indicates whether consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 <span data-ttu-id="a38e4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a38e4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a38e4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a38e4-106">Attributes and elements</span></span>

<span data-ttu-id="a38e4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a38e4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a38e4-108">属性</span><span class="sxs-lookup"><span data-stu-id="a38e4-108">Attributes</span></span>

<span data-ttu-id="a38e4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a38e4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a38e4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a38e4-110">Child elements</span></span>

<span data-ttu-id="a38e4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a38e4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a38e4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a38e4-112">Parent elements</span></span>

|<span data-ttu-id="a38e4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a38e4-113">**Element**</span></span>|<span data-ttu-id="a38e4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a38e4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a38e4-115">Mailヒント構成 (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="a38e4-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="a38e4-116">メールヒントサービスのサービス構成情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="a38e4-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a38e4-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a38e4-117">Text value</span></span>

<span data-ttu-id="a38e4-118">この要素のテキスト値は、 [Getmailtips ヒント操作](getmailtips-operation.md)のコンシューマーが、メッセージの宛先である外部受信者の数を示すメールヒントを表示する必要がある場合は**true**です。</span><span class="sxs-lookup"><span data-stu-id="a38e4-118">The text value of this element is **true** if consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> <span data-ttu-id="a38e4-119">[Getmailtips ヒント操作](getmailtips-operation.md)のコンシューマーが、メッセージの宛先である外部受信者の数を示すメールヒントを表示する必要がない場合は、値は**false**になります。</span><span class="sxs-lookup"><span data-stu-id="a38e4-119">The value is **false** if consumers of the [GetMailTips operation](getmailtips-operation.md) do not have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a38e4-120">注釈</span><span class="sxs-lookup"><span data-stu-id="a38e4-120">Remarks</span></span>

<span data-ttu-id="a38e4-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a38e4-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a38e4-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a38e4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a38e4-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="a38e4-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a38e4-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a38e4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a38e4-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a38e4-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="a38e4-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a38e4-126">Validation File</span></span>  <br/> |<span data-ttu-id="a38e4-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a38e4-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a38e4-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a38e4-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a38e4-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="a38e4-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a38e4-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="a38e4-130">See also</span></span>



[<span data-ttu-id="a38e4-131">GetMailTips ヒント操作</span><span class="sxs-lookup"><span data-stu-id="a38e4-131">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="a38e4-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a38e4-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

