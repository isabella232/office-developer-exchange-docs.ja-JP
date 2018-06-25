---
title: IsWritable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: IsWritable 要素は、基になっている取引先担当者または Active Directory の受信者に書き込むことがあるかどうかを指定します。
ms.openlocfilehash: 03f258d01ecfc12dfa4e09ac88f4a75340d2acf3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832158"
---
# <a name="iswritable"></a><span data-ttu-id="097eb-103">IsWritable</span><span class="sxs-lookup"><span data-stu-id="097eb-103">IsWritable</span></span>

<span data-ttu-id="097eb-104">**IsWritable**要素は、基になっている取引先担当者または Active Directory の受信者に書き込むことがあるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="097eb-104">The **IsWritable** element specifies whether the underlying contact or Active Directory recipient can be written to.</span></span> 
  
```XML
<IsWritable> true | false </IsWritable>
```

 <span data-ttu-id="097eb-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="097eb-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="097eb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="097eb-106">Attributes and elements</span></span>

<span data-ttu-id="097eb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="097eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="097eb-108">属性</span><span class="sxs-lookup"><span data-stu-id="097eb-108">Attributes</span></span>

<span data-ttu-id="097eb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="097eb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="097eb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="097eb-110">Child elements</span></span>

<span data-ttu-id="097eb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="097eb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="097eb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="097eb-112">Parent elements</span></span>

[<span data-ttu-id="097eb-113">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="097eb-113">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
  
## <a name="text-value"></a><span data-ttu-id="097eb-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="097eb-114">Text value</span></span>

<span data-ttu-id="097eb-115">**True** **IsWritable**要素のテキスト値は、取引先担当者または Active Directory オブジェクトは、書き込みアクセスに使用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="097eb-115">A text value of **true** for the **IsWritable** element indicates that the contact or Active Directory object is available for write access.</span></span> <span data-ttu-id="097eb-116">値が**false**のないことを示します、取引先担当者または Active Directory オブジェクトの書き込みアクセスに使用できます。</span><span class="sxs-lookup"><span data-stu-id="097eb-116">A value of **false** indicates that the contact or Active Directory object is not available for write access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="097eb-117">備考</span><span class="sxs-lookup"><span data-stu-id="097eb-117">Remarks</span></span>

<span data-ttu-id="097eb-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="097eb-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="097eb-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="097eb-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

