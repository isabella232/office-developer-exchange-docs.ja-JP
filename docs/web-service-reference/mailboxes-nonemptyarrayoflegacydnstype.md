---
title: メールボックス (NonEmptyArrayOfLegacyDNsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8e44bc49-8c99-472c-a507-0b5c25db9322
description: メールボックス要素は、従来の識別名で識別されたメールボックスの配列を指定します。
ms.openlocfilehash: 7e84a0d1c9ff53e45f8e844136f61de66f6d0ab4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465983"
---
# <a name="mailboxes-nonemptyarrayoflegacydnstype"></a><span data-ttu-id="db695-103">メールボックス (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="db695-103">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>

<span data-ttu-id="db695-104">**メールボックス**要素は、従来の識別名で識別されたメールボックスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="db695-104">The **Mailboxes** element specifies an array of mailboxes identified by legacy distinguished name.</span></span> 
  
```XML
<Mailboxes>
   <LegacyDN/>
</Mailboxes>
```

<span data-ttu-id="db695-105">**NonEmptyArrayofLegacyDNsType**</span><span class="sxs-lookup"><span data-stu-id="db695-105">**NonEmptyArrayofLegacyDNsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="db695-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="db695-106">Attributes and elements</span></span>

<span data-ttu-id="db695-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="db695-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db695-108">属性</span><span class="sxs-lookup"><span data-stu-id="db695-108">Attributes</span></span>

<span data-ttu-id="db695-109">なし。</span><span class="sxs-lookup"><span data-stu-id="db695-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db695-110">子要素</span><span class="sxs-lookup"><span data-stu-id="db695-110">Child elements</span></span>

[<span data-ttu-id="db695-111">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="db695-111">LegacyDN</span></span>](legacydn.md)
  
### <a name="parent-elements"></a><span data-ttu-id="db695-112">親要素</span><span class="sxs-lookup"><span data-stu-id="db695-112">Parent elements</span></span>

[<span data-ttu-id="db695-113">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="db695-113">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
  
## <a name="remarks"></a><span data-ttu-id="db695-114">注釈</span><span class="sxs-lookup"><span data-stu-id="db695-114">Remarks</span></span>

<span data-ttu-id="db695-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="db695-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="db695-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="db695-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db695-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="db695-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db695-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="db695-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="db695-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="db695-119">Schema name</span></span>  <br/> |<span data-ttu-id="db695-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="db695-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="db695-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="db695-121">Validation file</span></span>  <br/> |<span data-ttu-id="db695-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="db695-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="db695-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="db695-123">Can be empty</span></span>  <br/> ||
   

