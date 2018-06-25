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
description: IsContactPhoto 要素は、添付ファイルに連絡先の写真があるかどうかを示します。
ms.openlocfilehash: a015cd9bdb34ea9275952d5fe252a30cacf888ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831999"
---
# <a name="iscontactphoto"></a><span data-ttu-id="53a42-103">IsContactPhoto</span><span class="sxs-lookup"><span data-stu-id="53a42-103">IsContactPhoto</span></span>

<span data-ttu-id="53a42-104">**IsContactPhoto**要素は、添付ファイルに連絡先の写真があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="53a42-104">The **IsContactPhoto** element indicates whether the file attachment is a contact picture.</span></span> 
  
```xml
<IsContactPhoto>true or false</IsContactPhoto>
```

 <span data-ttu-id="53a42-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="53a42-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53a42-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="53a42-106">Attributes and elements</span></span>

<span data-ttu-id="53a42-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="53a42-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53a42-108">属性</span><span class="sxs-lookup"><span data-stu-id="53a42-108">Attributes</span></span>

<span data-ttu-id="53a42-109">なし。</span><span class="sxs-lookup"><span data-stu-id="53a42-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="53a42-110">子要素</span><span class="sxs-lookup"><span data-stu-id="53a42-110">Child elements</span></span>

<span data-ttu-id="53a42-111">なし。</span><span class="sxs-lookup"><span data-stu-id="53a42-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="53a42-112">親要素</span><span class="sxs-lookup"><span data-stu-id="53a42-112">Parent elements</span></span>

|<span data-ttu-id="53a42-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="53a42-113">**Element**</span></span>|<span data-ttu-id="53a42-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="53a42-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53a42-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="53a42-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="53a42-116">Exchange ストア内のアイテムに関連付けられているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="53a42-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="53a42-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="53a42-117">Text value</span></span>

<span data-ttu-id="53a42-118">この要素には、 **true**または**false**のいずれかができます。</span><span class="sxs-lookup"><span data-stu-id="53a42-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="53a42-119">既定値は、 **false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="53a42-119">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="53a42-120">備考</span><span class="sxs-lookup"><span data-stu-id="53a42-120">Remarks</span></span>

<span data-ttu-id="53a42-121">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="53a42-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="53a42-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="53a42-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53a42-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="53a42-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="53a42-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="53a42-124">Schema Name</span></span>  <br/> |<span data-ttu-id="53a42-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="53a42-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="53a42-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="53a42-126">Validation File</span></span>  <br/> |<span data-ttu-id="53a42-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="53a42-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="53a42-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="53a42-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="53a42-129">False</span><span class="sxs-lookup"><span data-stu-id="53a42-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="53a42-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="53a42-130">See also</span></span>



- [<span data-ttu-id="53a42-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="53a42-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

