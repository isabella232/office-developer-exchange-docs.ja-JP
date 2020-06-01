---
title: Entry (PhysicalAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: 9e5b6515-453e-4f4c-b55e-6ffefe23c31b
description: Entry 要素は、連絡先アイテムの単一の物理的なアドレスを記述します。
ms.openlocfilehash: 5e8343e9abebeeff8c2b81327b2e0f4ddcf45364
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459631"
---
# <a name="entry-physicaladdress"></a><span data-ttu-id="bf0c1-103">Entry (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="bf0c1-103">Entry (PhysicalAddress)</span></span>

<span data-ttu-id="bf0c1-104">**Entry**要素は、連絡先アイテムの単一の物理的なアドレスを記述します。</span><span class="sxs-lookup"><span data-stu-id="bf0c1-104">The **Entry** element describes a single physical address for a contact item.</span></span> 
  
```xml
<Entry Key="">
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
</Entry>
```

 <span data-ttu-id="bf0c1-105">**PhysicalAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="bf0c1-105">**PhysicalAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bf0c1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bf0c1-106">Attributes and elements</span></span>

<span data-ttu-id="bf0c1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bf0c1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf0c1-108">属性</span><span class="sxs-lookup"><span data-stu-id="bf0c1-108">Attributes</span></span>

|<span data-ttu-id="bf0c1-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="bf0c1-109">**Attribute**</span></span>|<span data-ttu-id="bf0c1-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="bf0c1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bf0c1-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="bf0c1-111">**Key**</span></span> <br/> | <span data-ttu-id="bf0c1-112">物理的な住所を識別します。</span><span class="sxs-lookup"><span data-stu-id="bf0c1-112">Identifies a physical address.</span></span><br/><br/> <span data-ttu-id="bf0c1-113">次に、この属性で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="bf0c1-113">The following are the possible values for this attribute:</span></span><br/>  <br/><span data-ttu-id="bf0c1-114">-Business</span><span class="sxs-lookup"><span data-stu-id="bf0c1-114">-  Business</span></span>  <br/><span data-ttu-id="bf0c1-115">-ホーム</span><span class="sxs-lookup"><span data-stu-id="bf0c1-115">-  Home</span></span>  <br/><span data-ttu-id="bf0c1-116">-その他</span><span class="sxs-lookup"><span data-stu-id="bf0c1-116">-  Other</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bf0c1-117">子要素</span><span class="sxs-lookup"><span data-stu-id="bf0c1-117">Child elements</span></span>

|<span data-ttu-id="bf0c1-118">**Element**</span><span class="sxs-lookup"><span data-stu-id="bf0c1-118">**Element**</span></span>|<span data-ttu-id="bf0c1-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="bf0c1-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf0c1-120">所在</span><span class="sxs-lookup"><span data-stu-id="bf0c1-120">Street</span></span>](street.md) <br/> |<span data-ttu-id="bf0c1-121">連絡先アイテムの住所を表します。</span><span class="sxs-lookup"><span data-stu-id="bf0c1-121">Represents a street address for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="bf0c1-122">市区町村</span><span class="sxs-lookup"><span data-stu-id="bf0c1-122">City</span></span>](city.md) <br/> |<span data-ttu-id="bf0c1-123">連絡先に関連付けられている市区町村名を表します。</span><span class="sxs-lookup"><span data-stu-id="bf0c1-123">Represents the city name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="bf0c1-124">State</span><span class="sxs-lookup"><span data-stu-id="bf0c1-124">State</span></span>](state-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bf0c1-125">連絡先アイテムの住居の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="bf0c1-125">Represents the state of residence for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="bf0c1-126">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="bf0c1-126">CountryOrRegion</span></span>](countryorregion.md) <br/> |<span data-ttu-id="bf0c1-127">指定された物理的な住所の国または地域を表します。</span><span class="sxs-lookup"><span data-stu-id="bf0c1-127">Represents the country or region for a given physical address.</span></span>  <br/> |
|[<span data-ttu-id="bf0c1-128">PostalCode</span><span class="sxs-lookup"><span data-stu-id="bf0c1-128">PostalCode</span></span>](postalcode.md) <br/> |<span data-ttu-id="bf0c1-129">連絡先アイテムの郵便番号を表します。</span><span class="sxs-lookup"><span data-stu-id="bf0c1-129">Represents the postal code for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bf0c1-130">親要素</span><span class="sxs-lookup"><span data-stu-id="bf0c1-130">Parent elements</span></span>

|<span data-ttu-id="bf0c1-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="bf0c1-131">**Element**</span></span>|<span data-ttu-id="bf0c1-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="bf0c1-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf0c1-133">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="bf0c1-133">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="bf0c1-134">連絡先に関連付けられている物理的な住所のコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="bf0c1-134">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bf0c1-135">注釈</span><span class="sxs-lookup"><span data-stu-id="bf0c1-135">Remarks</span></span>

<span data-ttu-id="bf0c1-136">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="bf0c1-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf0c1-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bf0c1-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf0c1-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="bf0c1-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bf0c1-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bf0c1-139">Schema Name</span></span>  <br/> |<span data-ttu-id="bf0c1-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="bf0c1-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="bf0c1-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bf0c1-141">Validation File</span></span>  <br/> |<span data-ttu-id="bf0c1-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="bf0c1-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bf0c1-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bf0c1-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="bf0c1-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="bf0c1-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf0c1-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="bf0c1-145">See also</span></span>

- [<span data-ttu-id="bf0c1-146">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="bf0c1-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="bf0c1-147">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="bf0c1-147">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="bf0c1-148">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="bf0c1-148">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="bf0c1-149">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="bf0c1-149">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

