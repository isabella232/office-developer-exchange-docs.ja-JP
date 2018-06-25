---
title: メールボックス (ArrayOfStringsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20596ebd-ed0f-4ad0-8631-e504220f1016
description: メールボックスの要素には、保留リストの影響を受けるメールボックスの一覧が含まれています。
ms.openlocfilehash: 8572c97d6de3045c4295ce39358c8acdc5eaea4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832279"
---
# <a name="mailboxes-arrayofstringstype"></a><span data-ttu-id="ff68d-103">メールボックス (ArrayOfStringsType)</span><span class="sxs-lookup"><span data-stu-id="ff68d-103">Mailboxes (ArrayOfStringsType)</span></span>

<span data-ttu-id="ff68d-104">**メールボックス**の要素には、保留リストの影響を受けるメールボックスの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ff68d-104">The **Mailboxes** element contains a list of mailboxes affected by the hold.</span></span> 
  
```XML
<Mailboxes>
   <String/>
</Mailboxes>
```

<span data-ttu-id="ff68d-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="ff68d-105">**ArrayOfStringsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ff68d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ff68d-106">Attributes and elements</span></span>

<span data-ttu-id="ff68d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ff68d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff68d-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff68d-108">Attributes</span></span>

<span data-ttu-id="ff68d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ff68d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff68d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ff68d-110">Child elements</span></span>

[<span data-ttu-id="ff68d-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ff68d-111">String</span></span>](string.md)
  
### <a name="parent-elements"></a><span data-ttu-id="ff68d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ff68d-112">Parent elements</span></span>

[<span data-ttu-id="ff68d-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ff68d-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="ff68d-114">備考</span><span class="sxs-lookup"><span data-stu-id="ff68d-114">Remarks</span></span>

<span data-ttu-id="ff68d-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ff68d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ff68d-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ff68d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff68d-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="ff68d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff68d-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="ff68d-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff68d-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ff68d-119">Schema name</span></span>  <br/> |<span data-ttu-id="ff68d-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ff68d-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff68d-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ff68d-121">Validation file</span></span>  <br/> |<span data-ttu-id="ff68d-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ff68d-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff68d-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ff68d-123">Can be empty</span></span>  <br/> ||
   

