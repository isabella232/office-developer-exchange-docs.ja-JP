---
title: メールボックス (PreviewItemMailboxType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e898d737-b6e4-4403-9c2c-aec52a48a83d
description: Mailbox 要素には、メールボックス識別子とユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスが含まれています。
ms.openlocfilehash: 4dc5ee45c00945c30a699daa0158c96679189ab1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463896"
---
# <a name="mailbox-previewitemmailboxtype"></a><span data-ttu-id="c4204-103">メールボックス (PreviewItemMailboxType)</span><span class="sxs-lookup"><span data-stu-id="c4204-103">Mailbox (PreviewItemMailboxType)</span></span>

<span data-ttu-id="c4204-104">**Mailbox**要素には、メールボックス識別子とユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c4204-104">The **Mailbox** element contains the mailbox identifier and the user's primary Simple Mail Transfer Protocol (SMTP) address.</span></span> 
  
```XML
<Mailbox>
   <MailboxId/>
   <PrimarySmtpAddress/>
</Mailbox>
```

<span data-ttu-id="c4204-105">**PreviewItemMailboxType**</span><span class="sxs-lookup"><span data-stu-id="c4204-105">**PreviewItemMailboxType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c4204-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c4204-106">Attributes and elements</span></span>

<span data-ttu-id="c4204-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c4204-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4204-108">属性</span><span class="sxs-lookup"><span data-stu-id="c4204-108">Attributes</span></span>

<span data-ttu-id="c4204-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c4204-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4204-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c4204-110">Child elements</span></span>

<span data-ttu-id="c4204-111">[MailboxId](mailboxid.md)  | [Primarysmtpaddress (文字列)](primarysmtpaddress-string.md)</span><span class="sxs-lookup"><span data-stu-id="c4204-111">[MailboxId](mailboxid.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c4204-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c4204-112">Parent elements</span></span>

[<span data-ttu-id="c4204-113">Searchプレビューアイテム</span><span class="sxs-lookup"><span data-stu-id="c4204-113">SearchPreviewItem</span></span>](searchpreviewitem.md)
  
## <a name="remarks"></a><span data-ttu-id="c4204-114">注釈</span><span class="sxs-lookup"><span data-stu-id="c4204-114">Remarks</span></span>

<span data-ttu-id="c4204-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c4204-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c4204-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c4204-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4204-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c4204-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4204-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="c4204-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c4204-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c4204-119">Schema name</span></span>  <br/> |<span data-ttu-id="c4204-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c4204-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="c4204-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c4204-121">Validation file</span></span>  <br/> |<span data-ttu-id="c4204-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c4204-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c4204-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c4204-123">Can be empty</span></span>  <br/> |<span data-ttu-id="c4204-124">false</span><span class="sxs-lookup"><span data-stu-id="c4204-124">false</span></span>  <br/> |
   

