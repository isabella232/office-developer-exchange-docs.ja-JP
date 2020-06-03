---
title: IsContactPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsContactPhoto
api_type:
- schema
ms.assetid: ae36b5f9-a787-4863-9dbc-258ad724801d
description: IsContactPhoto 要素は、添付ファイルが連絡先の画像であるかどうかを示します。
ms.openlocfilehash: f60e558ab4f20b59c1d5ae51f9dfca430feeff00
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455549"
---
# <a name="iscontactphoto"></a><span data-ttu-id="bb1eb-103">IsContactPhoto</span><span class="sxs-lookup"><span data-stu-id="bb1eb-103">IsContactPhoto</span></span>

<span data-ttu-id="bb1eb-104">**Iscontactphoto**要素は、添付ファイルが連絡先の画像であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bb1eb-104">The **IsContactPhoto** element indicates whether the file attachment is a contact picture.</span></span> 
  
```xml
<IsContactPhoto>true or false</IsContactPhoto>
```

 <span data-ttu-id="bb1eb-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="bb1eb-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb1eb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bb1eb-106">Attributes and elements</span></span>

<span data-ttu-id="bb1eb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bb1eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb1eb-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb1eb-108">Attributes</span></span>

<span data-ttu-id="bb1eb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bb1eb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb1eb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bb1eb-110">Child elements</span></span>

<span data-ttu-id="bb1eb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="bb1eb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bb1eb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bb1eb-112">Parent elements</span></span>

|<span data-ttu-id="bb1eb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="bb1eb-113">**Element**</span></span>|<span data-ttu-id="bb1eb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="bb1eb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb1eb-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="bb1eb-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="bb1eb-116">Exchange ストア内のアイテムに添付されているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="bb1eb-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bb1eb-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bb1eb-117">Text value</span></span>

<span data-ttu-id="bb1eb-118">この要素は、 **true**または**false**のいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="bb1eb-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="bb1eb-119">既定値は **false** です。</span><span class="sxs-lookup"><span data-stu-id="bb1eb-119">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bb1eb-120">注釈</span><span class="sxs-lookup"><span data-stu-id="bb1eb-120">Remarks</span></span>

<span data-ttu-id="bb1eb-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="bb1eb-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb1eb-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bb1eb-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb1eb-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="bb1eb-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bb1eb-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bb1eb-124">Schema Name</span></span>  <br/> |<span data-ttu-id="bb1eb-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="bb1eb-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="bb1eb-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bb1eb-126">Validation File</span></span>  <br/> |<span data-ttu-id="bb1eb-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="bb1eb-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bb1eb-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bb1eb-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="bb1eb-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="bb1eb-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb1eb-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="bb1eb-130">See also</span></span>



- [<span data-ttu-id="bb1eb-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="bb1eb-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

