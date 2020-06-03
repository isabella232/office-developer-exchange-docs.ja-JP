---
title: MailboxMoveEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 73d09137-d3bd-46b3-954a-a358ead07c91
description: MailBoxMoveEnabled 要素は、MailboxMoveEnabled () フラグを表します。 MailBoxMoveEnabled 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 4072d1c231e7cf109a39445fc44fbbb624f6f3a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530741"
---
# <a name="mailboxmoveenabled-soap"></a><span data-ttu-id="18234-105">MailboxMoveEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="18234-105">MailboxMoveEnabled (SOAP)</span></span>

<span data-ttu-id="18234-106">**MailBoxMoveEnabled**要素は、 **MailBoxMoveEnabled ()** フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="18234-106">The **MailBoxMoveEnabled** element represents the **MailboxMoveEnabled()** flag.</span></span> <span data-ttu-id="18234-107">**MailBoxMoveEnabled**要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="18234-107">The **MailBoxMoveEnabled** element is for internal use only.</span></span> <span data-ttu-id="18234-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="18234-108">This element is not used by clients.</span></span> 
  
```XML
<MailBoxMoveEnabled>true | false</MailBoxMoveEnabled>
```

<span data-ttu-id="18234-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="18234-109">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="18234-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="18234-110">Attributes and elements</span></span>

<span data-ttu-id="18234-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18234-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18234-112">属性</span><span class="sxs-lookup"><span data-stu-id="18234-112">Attributes</span></span>

<span data-ttu-id="18234-113">なし。</span><span class="sxs-lookup"><span data-stu-id="18234-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18234-114">子要素</span><span class="sxs-lookup"><span data-stu-id="18234-114">Child elements</span></span>

<span data-ttu-id="18234-115">なし。</span><span class="sxs-lookup"><span data-stu-id="18234-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="18234-116">親要素</span><span class="sxs-lookup"><span data-stu-id="18234-116">Parent elements</span></span>

|<span data-ttu-id="18234-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="18234-117">**Element**</span></span>|<span data-ttu-id="18234-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="18234-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18234-119">組織のリレーションシップ設定 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="18234-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="18234-120">1つの組織の組織上の関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="18234-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="18234-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="18234-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18234-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="18234-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="18234-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="18234-123">Schema Name</span></span>  <br/> |<span data-ttu-id="18234-124">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="18234-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="18234-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="18234-125">Validation File</span></span>  <br/> |<span data-ttu-id="18234-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="18234-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="18234-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="18234-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="18234-128">正しい</span><span class="sxs-lookup"><span data-stu-id="18234-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18234-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="18234-129">See also</span></span>

- [<span data-ttu-id="18234-130">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="18234-130">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

