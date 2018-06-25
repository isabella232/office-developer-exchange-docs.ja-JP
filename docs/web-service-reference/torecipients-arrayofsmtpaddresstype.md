---
title: ToRecipients (ArrayOfSmtpAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0e6fb89c-de19-48e7-af63-c41ebdf0b8e9
description: ToRecipients 要素は、アイテムを送信する受信者の一覧を指定します。
ms.openlocfilehash: dac2c80cfa964ca8e880e9be8a561c8e3ed09780
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839722"
---
# <a name="torecipients-arrayofsmtpaddresstype"></a><span data-ttu-id="26130-103">ToRecipients (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="26130-103">ToRecipients (ArrayOfSmtpAddressType)</span></span>

<span data-ttu-id="26130-104">**ToRecipients**要素は、アイテムを送信する受信者の一覧を指定します。</span><span class="sxs-lookup"><span data-stu-id="26130-104">The **ToRecipients** element specifies a list of recipients to whom the item was sent.</span></span> 
  
```XML
<ToRecipients>
   <SmtpAddress/>
</ToRecipients>
```

 <span data-ttu-id="26130-105">**ArrayOfSmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="26130-105">**ArrayOfSmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26130-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="26130-106">Attributes and elements</span></span>

<span data-ttu-id="26130-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="26130-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26130-108">属性</span><span class="sxs-lookup"><span data-stu-id="26130-108">Attributes</span></span>

<span data-ttu-id="26130-109">なし。</span><span class="sxs-lookup"><span data-stu-id="26130-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26130-110">子要素</span><span class="sxs-lookup"><span data-stu-id="26130-110">Child elements</span></span>

[<span data-ttu-id="26130-111">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="26130-111">SmtpAddress</span></span>](smtpaddress.md)
  
### <a name="parent-elements"></a><span data-ttu-id="26130-112">親要素</span><span class="sxs-lookup"><span data-stu-id="26130-112">Parent elements</span></span>

[<span data-ttu-id="26130-113">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="26130-113">SearchPreviewItem</span></span>](searchpreviewitem.md)
  
## <a name="remarks"></a><span data-ttu-id="26130-114">備考</span><span class="sxs-lookup"><span data-stu-id="26130-114">Remarks</span></span>

<span data-ttu-id="26130-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="26130-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="26130-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="26130-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26130-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="26130-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26130-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="26130-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26130-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="26130-119">Schema name</span></span>  <br/> |<span data-ttu-id="26130-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="26130-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="26130-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="26130-121">Validation file</span></span>  <br/> |<span data-ttu-id="26130-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="26130-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="26130-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="26130-123">Can be empty</span></span>  <br/> ||
   

