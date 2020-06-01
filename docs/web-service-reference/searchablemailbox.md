---
title: SearchableMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: SearchableMailbox 要素は、GetSearchableMailboxes 要求から返されるメールボックスを指定します。
ms.openlocfilehash: f790d9a707f10f64a776b2fc35255c233ad854b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467453"
---
# <a name="searchablemailbox"></a><span data-ttu-id="18af6-103">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="18af6-103">SearchableMailbox</span></span>

<span data-ttu-id="18af6-104">**SearchableMailbox**要素は、 **Getsearchablemailboxes**要求から返されるメールボックスを指定します。</span><span class="sxs-lookup"><span data-stu-id="18af6-104">The **SearchableMailbox** element specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<SearchableMailbox>
   <Guid/>
   <PrimarySmtpAddress/>
   <IsExternalMailbox/>
   <ExternalEmailAddress/>
   <DisplayName/>
   <IsMembershipGroup/>
   <ReferenceId/>
</SearchableMailbox>
```

 <span data-ttu-id="18af6-105">**SearchableMailboxType**</span><span class="sxs-lookup"><span data-stu-id="18af6-105">**SearchableMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18af6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="18af6-106">Attributes and elements</span></span>

<span data-ttu-id="18af6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18af6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18af6-108">属性</span><span class="sxs-lookup"><span data-stu-id="18af6-108">Attributes</span></span>

<span data-ttu-id="18af6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="18af6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18af6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="18af6-110">Child elements</span></span>

<span data-ttu-id="18af6-111">[Guid](guid-ex15websvcsotherref.md)  | [Primarysmtpaddress (文字列)](primarysmtpaddress-string.md)  | [IsExternalMailbox](isexternalmailbox.md)  | [ExternalEmailAddress](externalemailaddress.md)  | [DisplayName (文字列)](displayname-string.md)  | [Isメンバーシップグループ](ismembershipgroup.md)  | [ReferenceId](referenceid.md)</span><span class="sxs-lookup"><span data-stu-id="18af6-111">[Guid](guid-ex15websvcsotherref.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md) | [IsExternalMailbox](isexternalmailbox.md) | [ExternalEmailAddress](externalemailaddress.md) | [DisplayName (string)](displayname-string.md) | [IsMembershipGroup](ismembershipgroup.md) | [ReferenceId](referenceid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="18af6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="18af6-112">Parent elements</span></span>

[<span data-ttu-id="18af6-113">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="18af6-113">SearchableMailboxes</span></span>](searchablemailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="18af6-114">注釈</span><span class="sxs-lookup"><span data-stu-id="18af6-114">Remarks</span></span>

<span data-ttu-id="18af6-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="18af6-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="18af6-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="18af6-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18af6-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="18af6-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18af6-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="18af6-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18af6-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="18af6-119">Schema name</span></span>  <br/> |<span data-ttu-id="18af6-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="18af6-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="18af6-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="18af6-121">Validation file</span></span>  <br/> |<span data-ttu-id="18af6-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="18af6-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18af6-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="18af6-123">Can be empty</span></span>  <br/> ||
   

