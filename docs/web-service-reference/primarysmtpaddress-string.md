---
title: PrimarySmtpAddress (文字列)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 706c6387-c648-4ccc-85e6-12a07b66da2f
description: PrimarySmtpAddress 要素は、メールボックスのプライマリ簡易メール転送プロトコル (SMTP) アドレスを指定します。
ms.openlocfilehash: a103513c7cac94bd4923c12ed402b81c5d794e1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832878"
---
# <a name="primarysmtpaddress-string"></a><span data-ttu-id="2fe3a-103">PrimarySmtpAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="2fe3a-103">PrimarySmtpAddress (string)</span></span>

<span data-ttu-id="2fe3a-104">**PrimarySmtpAddress**要素は、メールボックスのプライマリ簡易メール転送プロトコル (SMTP) アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="2fe3a-104">The **PrimarySmtpAddress** element specifies the primary Simple Mail Transfer Protocol (SMTP) address of the mailbox.</span></span> 
  
```XML
<PrimarySmtpAddress></PrimarySmtpAddress>
```

 <span data-ttu-id="2fe3a-105">**string**</span><span class="sxs-lookup"><span data-stu-id="2fe3a-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2fe3a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2fe3a-106">Attributes and elements</span></span>

<span data-ttu-id="2fe3a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2fe3a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2fe3a-108">属性</span><span class="sxs-lookup"><span data-stu-id="2fe3a-108">Attributes</span></span>

<span data-ttu-id="2fe3a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2fe3a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2fe3a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2fe3a-110">Child elements</span></span>

<span data-ttu-id="2fe3a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2fe3a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2fe3a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2fe3a-112">Parent elements</span></span>

<span data-ttu-id="2fe3a-113">[ユーザー Id (文字列)](userid-string.md) | [メールボックス (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [SearchableMailbox](searchablemailbox.md)</span><span class="sxs-lookup"><span data-stu-id="2fe3a-113">[UserId (string)](userid-string.md) | [Mailbox (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [SearchableMailbox](searchablemailbox.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2fe3a-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2fe3a-114">Text value</span></span>

<span data-ttu-id="2fe3a-115">**PrimarySmtpAddress**要素のテキスト値は、メールボックスのプライマリ SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="2fe3a-115">The text value of the **PrimarySmtpAddress** element is the primary SMTP address of the mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2fe3a-116">備考</span><span class="sxs-lookup"><span data-stu-id="2fe3a-116">Remarks</span></span>

<span data-ttu-id="2fe3a-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2fe3a-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2fe3a-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2fe3a-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2fe3a-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="2fe3a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2fe3a-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="2fe3a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2fe3a-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2fe3a-121">Schema name</span></span>  <br/> |<span data-ttu-id="2fe3a-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2fe3a-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="2fe3a-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2fe3a-123">Validation file</span></span>  <br/> |<span data-ttu-id="2fe3a-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2fe3a-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2fe3a-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2fe3a-125">Can be empty</span></span>  <br/> ||
   

