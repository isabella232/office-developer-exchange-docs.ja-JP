---
title: メールボックス (PreviewItemMailboxType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e898d737-b6e4-4403-9c2c-aec52a48a83d
description: メールボックスの要素には、メールボックス id およびユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスが含まれています。
ms.openlocfilehash: 1b6669928015bc880806479d294a4063034a559f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832255"
---
# <a name="mailbox-previewitemmailboxtype"></a><span data-ttu-id="bde28-103">メールボックス (PreviewItemMailboxType)</span><span class="sxs-lookup"><span data-stu-id="bde28-103">Mailbox (PreviewItemMailboxType)</span></span>

<span data-ttu-id="bde28-104">**メールボックス**の要素には、メールボックス id およびユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bde28-104">The **Mailbox** element contains the mailbox identifier and the user's primary Simple Mail Transfer Protocol (SMTP) address.</span></span> 
  
```XML
<Mailbox>
   <MailboxId/>
   <PrimarySmtpAddress/>
</Mailbox>
```

<span data-ttu-id="bde28-105">**PreviewItemMailboxType**</span><span class="sxs-lookup"><span data-stu-id="bde28-105">**PreviewItemMailboxType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bde28-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bde28-106">Attributes and elements</span></span>

<span data-ttu-id="bde28-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bde28-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bde28-108">属性</span><span class="sxs-lookup"><span data-stu-id="bde28-108">Attributes</span></span>

<span data-ttu-id="bde28-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bde28-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bde28-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bde28-110">Child elements</span></span>

<span data-ttu-id="bde28-111">[MailboxId](mailboxid.md) | [PrimarySmtpAddress (文字列)](primarysmtpaddress-string.md)</span><span class="sxs-lookup"><span data-stu-id="bde28-111">[MailboxId](mailboxid.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bde28-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bde28-112">Parent elements</span></span>

[<span data-ttu-id="bde28-113">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="bde28-113">SearchPreviewItem</span></span>](searchpreviewitem.md)
  
## <a name="remarks"></a><span data-ttu-id="bde28-114">備考</span><span class="sxs-lookup"><span data-stu-id="bde28-114">Remarks</span></span>

<span data-ttu-id="bde28-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bde28-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bde28-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bde28-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bde28-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="bde28-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bde28-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="bde28-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bde28-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bde28-119">Schema name</span></span>  <br/> |<span data-ttu-id="bde28-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="bde28-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="bde28-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bde28-121">Validation file</span></span>  <br/> |<span data-ttu-id="bde28-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bde28-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bde28-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bde28-123">Can be empty</span></span>  <br/> |<span data-ttu-id="bde28-124">false</span><span class="sxs-lookup"><span data-stu-id="bde28-124">false</span></span>  <br/> |
   

