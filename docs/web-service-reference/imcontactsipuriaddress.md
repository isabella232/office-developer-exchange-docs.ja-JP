---
title: ImContactSipUriAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4a3d12a2-0736-4f60-b3b8-14586467df3c
description: ImContactSipUriAddress 要素には、インスタント メッセージング (IM) グループに追加される連絡先の SIP URI のアドレスが含まれています。
ms.openlocfilehash: 230f663c10f5738707a8d03a2ba6be8a4e6d285a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831886"
---
# <a name="imcontactsipuriaddress"></a><span data-ttu-id="7d5ac-103">ImContactSipUriAddress</span><span class="sxs-lookup"><span data-stu-id="7d5ac-103">ImContactSipUriAddress</span></span>

<span data-ttu-id="7d5ac-104">**ImContactSipUriAddress**要素には、インスタント メッセージング (IM) グループに追加される連絡先の SIP URI のアドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7d5ac-104">The **ImContactSipUriAddress** element contains the SIP URI address of a contact that is added to an instant messaging (IM) group.</span></span> 
  
```XML
<ImContactSipUriAddress></ImContactSipUriAddress>
```

 <span data-ttu-id="7d5ac-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="7d5ac-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d5ac-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7d5ac-106">Attributes and elements</span></span>

<span data-ttu-id="7d5ac-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7d5ac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d5ac-108">属性</span><span class="sxs-lookup"><span data-stu-id="7d5ac-108">Attributes</span></span>

<span data-ttu-id="7d5ac-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7d5ac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d5ac-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7d5ac-110">Child elements</span></span>

<span data-ttu-id="7d5ac-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7d5ac-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7d5ac-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7d5ac-112">Parent elements</span></span>

[<span data-ttu-id="7d5ac-113">AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="7d5ac-113">AddNewTelUriContactToGroup</span></span>](addnewteluricontacttogroup.md)
  
## <a name="text-value"></a><span data-ttu-id="7d5ac-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7d5ac-114">Text value</span></span>

<span data-ttu-id="7d5ac-115">**ImContactSipUriAddress**要素のテキスト値は、連絡先の SIP URI アドレスです。</span><span class="sxs-lookup"><span data-stu-id="7d5ac-115">The text value of the **ImContactSipUriAddress** element is the SIP URI address of a contact.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7d5ac-116">備考</span><span class="sxs-lookup"><span data-stu-id="7d5ac-116">Remarks</span></span>

<span data-ttu-id="7d5ac-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7d5ac-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7d5ac-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7d5ac-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d5ac-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="7d5ac-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d5ac-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="7d5ac-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7d5ac-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7d5ac-121">Schema name</span></span>  <br/> |<span data-ttu-id="7d5ac-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7d5ac-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7d5ac-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7d5ac-123">Validation file</span></span>  <br/> |<span data-ttu-id="7d5ac-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7d5ac-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7d5ac-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7d5ac-125">Can be empty</span></span>  <br/> |<span data-ttu-id="7d5ac-126">いいえ</span><span class="sxs-lookup"><span data-stu-id="7d5ac-126">False</span></span>  <br/> |
   

