---
title: メールボックス (ArrayOfStringsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20596ebd-ed0f-4ad0-8631-e504220f1016
description: メールボックス要素には、保留の影響を受けるメールボックスの一覧が含まれています。
ms.openlocfilehash: 376bd1f007e4b3d27bc44076a7b09993c49bd416
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468160"
---
# <a name="mailboxes-arrayofstringstype"></a><span data-ttu-id="64aff-103">メールボックス (ArrayOfStringsType)</span><span class="sxs-lookup"><span data-stu-id="64aff-103">Mailboxes (ArrayOfStringsType)</span></span>

<span data-ttu-id="64aff-104">**メールボックス**要素には、保留の影響を受けるメールボックスの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="64aff-104">The **Mailboxes** element contains a list of mailboxes affected by the hold.</span></span> 
  
```XML
<Mailboxes>
   <String/>
</Mailboxes>
```

<span data-ttu-id="64aff-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="64aff-105">**ArrayOfStringsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="64aff-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="64aff-106">Attributes and elements</span></span>

<span data-ttu-id="64aff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="64aff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64aff-108">属性</span><span class="sxs-lookup"><span data-stu-id="64aff-108">Attributes</span></span>

<span data-ttu-id="64aff-109">なし。</span><span class="sxs-lookup"><span data-stu-id="64aff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64aff-110">子要素</span><span class="sxs-lookup"><span data-stu-id="64aff-110">Child elements</span></span>

[<span data-ttu-id="64aff-111">String</span><span class="sxs-lookup"><span data-stu-id="64aff-111">String</span></span>](string.md)
  
### <a name="parent-elements"></a><span data-ttu-id="64aff-112">親要素</span><span class="sxs-lookup"><span data-stu-id="64aff-112">Parent elements</span></span>

[<span data-ttu-id="64aff-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="64aff-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="64aff-114">注釈</span><span class="sxs-lookup"><span data-stu-id="64aff-114">Remarks</span></span>

<span data-ttu-id="64aff-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="64aff-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="64aff-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="64aff-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64aff-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="64aff-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64aff-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="64aff-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="64aff-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="64aff-119">Schema name</span></span>  <br/> |<span data-ttu-id="64aff-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="64aff-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="64aff-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="64aff-121">Validation file</span></span>  <br/> |<span data-ttu-id="64aff-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="64aff-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="64aff-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="64aff-123">Can be empty</span></span>  <br/> ||
   

