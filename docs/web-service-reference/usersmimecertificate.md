---
title: UserSMIMECertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 66e6b4ba-368d-4469-bd47-e59441b7d64d
description: UserSMIMECertificate 要素には、連絡先の SMIME 証明書をエンコードする値が含まれています。
ms.openlocfilehash: 7e2dbc6a9c8b04758ba99db036e237d8837850aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467656"
---
# <a name="usersmimecertificate"></a><span data-ttu-id="9b835-103">UserSMIMECertificate</span><span class="sxs-lookup"><span data-stu-id="9b835-103">UserSMIMECertificate</span></span>

<span data-ttu-id="9b835-104">**UserSMIMECertificate**要素には、連絡先の SMIME 証明書をエンコードする値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9b835-104">The **UserSMIMECertificate** element contains a value that encodes a contact's SMIME certificate.</span></span> 
  
```XML
<UserSMIMECertificate/>
```

 <span data-ttu-id="9b835-105">**ArrayOfBinaryType**</span><span class="sxs-lookup"><span data-stu-id="9b835-105">**ArrayOfBinaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b835-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9b835-106">Attributes and elements</span></span>

<span data-ttu-id="9b835-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9b835-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b835-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b835-108">Attributes</span></span>

<span data-ttu-id="9b835-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9b835-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b835-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9b835-110">Child elements</span></span>

|<span data-ttu-id="9b835-111">**要素名**</span><span class="sxs-lookup"><span data-stu-id="9b835-111">**Element name**</span></span>|<span data-ttu-id="9b835-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9b835-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b835-113">Base64Binary</span><span class="sxs-lookup"><span data-stu-id="9b835-113">Base64Binary</span></span>](base64binary.md) <br/> |<span data-ttu-id="9b835-114">Base64 でエンコードされた値を格納します。</span><span class="sxs-lookup"><span data-stu-id="9b835-114">Contains a Base64-encoded value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b835-115">親要素</span><span class="sxs-lookup"><span data-stu-id="9b835-115">Parent elements</span></span>

|<span data-ttu-id="9b835-116">**要素名**</span><span class="sxs-lookup"><span data-stu-id="9b835-116">**Element name**</span></span>|<span data-ttu-id="9b835-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="9b835-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b835-118">連絡先</span><span class="sxs-lookup"><span data-stu-id="9b835-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="9b835-119">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="9b835-119">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9b835-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9b835-120">Text value</span></span>

<span data-ttu-id="9b835-121">なし。</span><span class="sxs-lookup"><span data-stu-id="9b835-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9b835-122">注釈</span><span class="sxs-lookup"><span data-stu-id="9b835-122">Remarks</span></span>

<span data-ttu-id="9b835-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9b835-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="9b835-124">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9b835-124">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b835-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9b835-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b835-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="9b835-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b835-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9b835-127">Schema name</span></span>  <br/> |<span data-ttu-id="9b835-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9b835-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="9b835-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9b835-129">Validation file</span></span>  <br/> |<span data-ttu-id="9b835-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9b835-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b835-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9b835-131">Can be empty</span></span>  <br/> |<span data-ttu-id="9b835-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="9b835-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b835-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="9b835-133">See also</span></span>



- [<span data-ttu-id="9b835-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9b835-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="9b835-135">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="9b835-135">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

