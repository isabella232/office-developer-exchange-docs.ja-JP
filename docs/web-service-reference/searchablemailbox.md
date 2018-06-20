---
title: SearchableMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: SearchableMailbox 要素は、メールボックスは、GetSearchableMailboxes 要求から返されるを指定します。
ms.openlocfilehash: 0d0981d050fa388e83eaa8408b60d305296c1f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833284"
---
# <a name="searchablemailbox"></a><span data-ttu-id="8f396-103">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="8f396-103">SearchableMailbox</span></span>

<span data-ttu-id="8f396-104">**SearchableMailbox**要素は、メールボックスは、 **GetSearchableMailboxes**要求から返されるを指定します。</span><span class="sxs-lookup"><span data-stu-id="8f396-104">The **SearchableMailbox** element specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span> 
  
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

 <span data-ttu-id="8f396-105">**SearchableMailboxType**</span><span class="sxs-lookup"><span data-stu-id="8f396-105">**SearchableMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8f396-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8f396-106">Attributes and elements</span></span>

<span data-ttu-id="8f396-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8f396-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f396-108">属性</span><span class="sxs-lookup"><span data-stu-id="8f396-108">Attributes</span></span>

<span data-ttu-id="8f396-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8f396-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8f396-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8f396-110">Child elements</span></span>

<span data-ttu-id="8f396-111">[Guid](guid-ex15websvcsotherref.md) | [PrimarySmtpAddress (文字列)](primarysmtpaddress-string.md) | [IsExternalMailbox](isexternalmailbox.md) | [ExternalEmailAddress](externalemailaddress.md) | [表示名 (文字列)](displayname-string.md) | [IsMembershipGroup](ismembershipgroup.md)  |  [参照 id が](referenceid.md)</span><span class="sxs-lookup"><span data-stu-id="8f396-111">[Guid](guid-ex15websvcsotherref.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md) | [IsExternalMailbox](isexternalmailbox.md) | [ExternalEmailAddress](externalemailaddress.md) | [DisplayName (string)](displayname-string.md) | [IsMembershipGroup](ismembershipgroup.md) | [ReferenceId](referenceid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8f396-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8f396-112">Parent elements</span></span>

[<span data-ttu-id="8f396-113">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="8f396-113">SearchableMailboxes</span></span>](searchablemailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="8f396-114">備考</span><span class="sxs-lookup"><span data-stu-id="8f396-114">Remarks</span></span>

<span data-ttu-id="8f396-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8f396-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8f396-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8f396-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8f396-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="8f396-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f396-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="8f396-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8f396-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8f396-119">Schema name</span></span>  <br/> |<span data-ttu-id="8f396-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8f396-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="8f396-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8f396-121">Validation file</span></span>  <br/> |<span data-ttu-id="8f396-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8f396-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8f396-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8f396-123">Can be empty</span></span>  <br/> ||
   

