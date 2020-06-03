---
title: '[Senders (送信者)]'
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 69d88bb1-397c-4fb8-bd2b-21cccc5bb35d
description: '[送信者] 要素は、SMTP (Simple Mail Transfer Protocol) アドレスの配列を指定します。'
ms.openlocfilehash: 125d448be53b2ae297cd1e7249a04da6eda5d960
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530573"
---
# <a name="senders"></a><span data-ttu-id="1fb91-103">[Senders (送信者)]</span><span class="sxs-lookup"><span data-stu-id="1fb91-103">Senders</span></span>

<span data-ttu-id="1fb91-104">[**送信者**] 要素は、SMTP (Simple Mail Transfer Protocol) アドレスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="1fb91-104">The **Senders** element specifies an array of Simple Mail Transfer Protocol (SMTP) addresses.</span></span> 
  
```XML
<Senders>
   <SmtpAddress/>
</Senders>
```

 <span data-ttu-id="1fb91-105">**ArrayOfSmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="1fb91-105">**ArrayOfSmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1fb91-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1fb91-106">Attributes and elements</span></span>

<span data-ttu-id="1fb91-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1fb91-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1fb91-108">属性</span><span class="sxs-lookup"><span data-stu-id="1fb91-108">Attributes</span></span>

<span data-ttu-id="1fb91-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1fb91-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1fb91-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1fb91-110">Child elements</span></span>

[<span data-ttu-id="1fb91-111">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1fb91-111">SmtpAddress</span></span>](smtpaddress.md)
  
### <a name="parent-elements"></a><span data-ttu-id="1fb91-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1fb91-112">Parent elements</span></span>

[<span data-ttu-id="1fb91-113">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="1fb91-113">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md)
  
## <a name="remarks"></a><span data-ttu-id="1fb91-114">注釈</span><span class="sxs-lookup"><span data-stu-id="1fb91-114">Remarks</span></span>

<span data-ttu-id="1fb91-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1fb91-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1fb91-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1fb91-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1fb91-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1fb91-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1fb91-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="1fb91-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1fb91-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1fb91-119">Schema name</span></span>  <br/> |<span data-ttu-id="1fb91-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1fb91-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="1fb91-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1fb91-121">Validation file</span></span>  <br/> |<span data-ttu-id="1fb91-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1fb91-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1fb91-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1fb91-123">Can be empty</span></span>  <br/> ||
   

