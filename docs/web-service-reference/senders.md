---
title: 送信者
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 69d88bb1-397c-4fb8-bd2b-21cccc5bb35d
description: 送信者要素では、簡易メール転送プロトコル (SMTP) アドレスの配列を指定します。
ms.openlocfilehash: 0794b042c00183d56b2fb2aefe8587e0fdf1344d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833329"
---
# <a name="senders"></a><span data-ttu-id="8bf5e-103">送信者</span><span class="sxs-lookup"><span data-stu-id="8bf5e-103">Senders</span></span>

<span data-ttu-id="8bf5e-104">**送信者**要素では、簡易メール転送プロトコル (SMTP) アドレスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bf5e-104">The **Senders** element specifies an array of Simple Mail Transfer Protocol (SMTP) addresses.</span></span> 
  
```XML
<Senders>
   <SmtpAddress/>
</Senders>
```

 <span data-ttu-id="8bf5e-105">**ArrayOfSmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="8bf5e-105">**ArrayOfSmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8bf5e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8bf5e-106">Attributes and elements</span></span>

<span data-ttu-id="8bf5e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8bf5e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8bf5e-108">属性</span><span class="sxs-lookup"><span data-stu-id="8bf5e-108">Attributes</span></span>

<span data-ttu-id="8bf5e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8bf5e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8bf5e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8bf5e-110">Child elements</span></span>

[<span data-ttu-id="8bf5e-111">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="8bf5e-111">SmtpAddress</span></span>](smtpaddress.md)
  
### <a name="parent-elements"></a><span data-ttu-id="8bf5e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8bf5e-112">Parent elements</span></span>

[<span data-ttu-id="8bf5e-113">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="8bf5e-113">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md)
  
## <a name="remarks"></a><span data-ttu-id="8bf5e-114">備考</span><span class="sxs-lookup"><span data-stu-id="8bf5e-114">Remarks</span></span>

<span data-ttu-id="8bf5e-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8bf5e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8bf5e-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8bf5e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8bf5e-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="8bf5e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8bf5e-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="8bf5e-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8bf5e-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8bf5e-119">Schema name</span></span>  <br/> |<span data-ttu-id="8bf5e-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8bf5e-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="8bf5e-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8bf5e-121">Validation file</span></span>  <br/> |<span data-ttu-id="8bf5e-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8bf5e-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8bf5e-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8bf5e-123">Can be empty</span></span>  <br/> ||
   

