---
title: IsWritable 可能
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: IsWritable 可能要素は、基になる連絡先または Active Directory 受信者に書き込むことができるかどうかを指定します。
ms.openlocfilehash: 96075adc1772027456f8829eee43bdc734644c09
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467572"
---
# <a name="iswritable"></a><span data-ttu-id="6c5d4-103">IsWritable 可能</span><span class="sxs-lookup"><span data-stu-id="6c5d4-103">IsWritable</span></span>

<span data-ttu-id="6c5d4-104">**Iswritable 可能**要素は、基になる連絡先または Active Directory 受信者に書き込むことができるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6c5d4-104">The **IsWritable** element specifies whether the underlying contact or Active Directory recipient can be written to.</span></span> 
  
```XML
<IsWritable> true | false </IsWritable>
```

 <span data-ttu-id="6c5d4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6c5d4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c5d4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6c5d4-106">Attributes and elements</span></span>

<span data-ttu-id="6c5d4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c5d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c5d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="6c5d4-108">Attributes</span></span>

<span data-ttu-id="6c5d4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6c5d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c5d4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6c5d4-110">Child elements</span></span>

<span data-ttu-id="6c5d4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6c5d4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c5d4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6c5d4-112">Parent elements</span></span>

[<span data-ttu-id="6c5d4-113">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="6c5d4-113">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
  
## <a name="text-value"></a><span data-ttu-id="6c5d4-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6c5d4-114">Text value</span></span>

<span data-ttu-id="6c5d4-115">**Iswritable**要素のテキスト値が**true**の場合は、連絡先または Active Directory オブジェクトが書き込みアクセスで利用可能であることを示します。</span><span class="sxs-lookup"><span data-stu-id="6c5d4-115">A text value of **true** for the **IsWritable** element indicates that the contact or Active Directory object is available for write access.</span></span> <span data-ttu-id="6c5d4-116">値が**false**の場合は、連絡先または Active Directory オブジェクトが書き込みアクセスで利用できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="6c5d4-116">A value of **false** indicates that the contact or Active Directory object is not available for write access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6c5d4-117">注釈</span><span class="sxs-lookup"><span data-stu-id="6c5d4-117">Remarks</span></span>

<span data-ttu-id="6c5d4-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6c5d4-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6c5d4-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6c5d4-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

