---
title: エントリ (PhysicalAddress)
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
description: エントリ要素は、連絡先アイテムの 1 つの物理アドレスについて説明します。
ms.openlocfilehash: 4551e6117e5f91d901fe160f37e8f67cb1bc5ac7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760311"
---
# <a name="entry-physicaladdress"></a><span data-ttu-id="dbea2-103">エントリ (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="dbea2-103">Entry (PhysicalAddress)</span></span>

<span data-ttu-id="dbea2-104">**エントリ**要素は、連絡先アイテムの 1 つの物理アドレスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="dbea2-104">The **Entry** element describes a single physical address for a contact item.</span></span> 
  
```xml
<Entry Key="">
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
</Entry>
```

 <span data-ttu-id="dbea2-105">**PhysicalAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="dbea2-105">**PhysicalAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dbea2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dbea2-106">Attributes and elements</span></span>

<span data-ttu-id="dbea2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dbea2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbea2-108">属性</span><span class="sxs-lookup"><span data-stu-id="dbea2-108">Attributes</span></span>

|<span data-ttu-id="dbea2-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="dbea2-109">**Attribute**</span></span>|<span data-ttu-id="dbea2-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="dbea2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dbea2-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="dbea2-111">**Key**</span></span> <br/> | <span data-ttu-id="dbea2-112">物理アドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="dbea2-112">Identifies a physical address.</span></span><br/><br/> <span data-ttu-id="dbea2-113">次に、この属性で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="dbea2-113">The following are the possible values for this attribute:</span></span><br/>  <br/><span data-ttu-id="dbea2-114">ビジネス</span><span class="sxs-lookup"><span data-stu-id="dbea2-114">-  Business</span></span>  <br/><span data-ttu-id="dbea2-115">-ホーム</span><span class="sxs-lookup"><span data-stu-id="dbea2-115">-  Home</span></span>  <br/><span data-ttu-id="dbea2-116">-その他の</span><span class="sxs-lookup"><span data-stu-id="dbea2-116">-  Other</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dbea2-117">子要素</span><span class="sxs-lookup"><span data-stu-id="dbea2-117">Child elements</span></span>

|<span data-ttu-id="dbea2-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="dbea2-118">**Element**</span></span>|<span data-ttu-id="dbea2-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="dbea2-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbea2-120">番地</span><span class="sxs-lookup"><span data-stu-id="dbea2-120">Street</span></span>](street.md) <br/> |<span data-ttu-id="dbea2-121">連絡先アイテムの所在地の住所を表します。</span><span class="sxs-lookup"><span data-stu-id="dbea2-121">Represents a street address for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="dbea2-122">City</span><span class="sxs-lookup"><span data-stu-id="dbea2-122">City</span></span>](city.md) <br/> |<span data-ttu-id="dbea2-123">連絡先に関連付けられている市区町村名を表します。</span><span class="sxs-lookup"><span data-stu-id="dbea2-123">Represents the city name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="dbea2-124">State</span><span class="sxs-lookup"><span data-stu-id="dbea2-124">State</span></span>](state-ex15websvcsotherref.md) <br/> |<span data-ttu-id="dbea2-125">連絡先アイテムの居住地の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="dbea2-125">Represents the state of residence for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="dbea2-126">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="dbea2-126">CountryOrRegion</span></span>](countryorregion.md) <br/> |<span data-ttu-id="dbea2-127">国または地域の特定の物理アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="dbea2-127">Represents the country or region for a given physical address.</span></span>  <br/> |
|<span data-ttu-id="dbea2-128">[[郵便番号]](postalcode.md)</span><span class="sxs-lookup"><span data-stu-id="dbea2-128">[PostalCode](postalcode.md)</span></span> <br/> |<span data-ttu-id="dbea2-129">連絡先アイテムの郵便番号コードを表します。</span><span class="sxs-lookup"><span data-stu-id="dbea2-129">Represents the postal code for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dbea2-130">親要素</span><span class="sxs-lookup"><span data-stu-id="dbea2-130">Parent elements</span></span>

|<span data-ttu-id="dbea2-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="dbea2-131">**Element**</span></span>|<span data-ttu-id="dbea2-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="dbea2-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbea2-133">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="dbea2-133">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="dbea2-134">連絡先に関連付けられている物理アドレスのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="dbea2-134">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dbea2-135">備考</span><span class="sxs-lookup"><span data-stu-id="dbea2-135">Remarks</span></span>

<span data-ttu-id="dbea2-136">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="dbea2-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dbea2-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="dbea2-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dbea2-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="dbea2-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dbea2-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dbea2-139">Schema Name</span></span>  <br/> |<span data-ttu-id="dbea2-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="dbea2-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="dbea2-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dbea2-141">Validation File</span></span>  <br/> |<span data-ttu-id="dbea2-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dbea2-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dbea2-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dbea2-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="dbea2-144">False</span><span class="sxs-lookup"><span data-stu-id="dbea2-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dbea2-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="dbea2-145">See also</span></span>

- [<span data-ttu-id="dbea2-146">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dbea2-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="dbea2-147">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="dbea2-147">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="dbea2-148">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="dbea2-148">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="dbea2-149">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="dbea2-149">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

