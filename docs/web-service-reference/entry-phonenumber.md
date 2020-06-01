---
title: Entry (PhoneNumber)
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
ms.assetid: e3d0a4d5-8af8-4607-aa2e-ef3111b63b55
description: Entry 要素は、連絡先の電話番号を表します。
ms.openlocfilehash: 62f7091bb750dc7ca74b1e5637a437e2cdad4f1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459638"
---
# <a name="entry-phonenumber"></a><span data-ttu-id="66b2d-103">Entry (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="66b2d-103">Entry (PhoneNumber)</span></span>

<span data-ttu-id="66b2d-104">**Entry**要素は、連絡先の電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="66b2d-104">The **Entry** element represents a telephone number for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="66b2d-105">**PhoneNumberDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="66b2d-105">**PhoneNumberDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66b2d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="66b2d-106">Attributes and elements</span></span>

<span data-ttu-id="66b2d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="66b2d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66b2d-108">属性</span><span class="sxs-lookup"><span data-stu-id="66b2d-108">Attributes</span></span>

|<span data-ttu-id="66b2d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="66b2d-109">**Attribute**</span></span>|<span data-ttu-id="66b2d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="66b2d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="66b2d-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="66b2d-111">**Key**</span></span> <br/> | <span data-ttu-id="66b2d-112">電話番号を識別します。</span><span class="sxs-lookup"><span data-stu-id="66b2d-112">Identifies the telephone number.</span></span> <span data-ttu-id="66b2d-113">キー属性の型は**PhoneNumberKeyType**です。</span><span class="sxs-lookup"><span data-stu-id="66b2d-113">The Key attribute is of type **PhoneNumberKeyType**.</span></span><br/><br/> <span data-ttu-id="66b2d-114">次に、この属性で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="66b2d-114">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="66b2d-115">- AssistantPhone</span><span class="sxs-lookup"><span data-stu-id="66b2d-115">-  AssistantPhone</span></span>  <br/><span data-ttu-id="66b2d-116">-BusinessFax</span><span class="sxs-lookup"><span data-stu-id="66b2d-116">-  BusinessFax</span></span>  <br/><span data-ttu-id="66b2d-117">- BusinessPhone</span><span class="sxs-lookup"><span data-stu-id="66b2d-117">-  BusinessPhone</span></span>  <br/><span data-ttu-id="66b2d-118">- BusinessPhone2</span><span class="sxs-lookup"><span data-stu-id="66b2d-118">-  BusinessPhone2</span></span>  <br/><span data-ttu-id="66b2d-119">-コールバック</span><span class="sxs-lookup"><span data-stu-id="66b2d-119">-  Callback</span></span>  <br/><span data-ttu-id="66b2d-120">-CarPhone</span><span class="sxs-lookup"><span data-stu-id="66b2d-120">-  CarPhone</span></span>  <br/><span data-ttu-id="66b2d-121">-会社の Mainphone</span><span class="sxs-lookup"><span data-stu-id="66b2d-121">-  CompanyMainPhone</span></span>  <br/><span data-ttu-id="66b2d-122">-ホーム Fax</span><span class="sxs-lookup"><span data-stu-id="66b2d-122">-  HomeFax</span></span>  <br/><span data-ttu-id="66b2d-123">-HomePhone</span><span class="sxs-lookup"><span data-stu-id="66b2d-123">-  HomePhone</span></span>  <br/><span data-ttu-id="66b2d-124">- HomePhone2</span><span class="sxs-lookup"><span data-stu-id="66b2d-124">-  HomePhone2</span></span>  <br/><span data-ttu-id="66b2d-125">-Isdn</span><span class="sxs-lookup"><span data-stu-id="66b2d-125">-  Isdn</span></span>  <br/><span data-ttu-id="66b2d-126">-MobilePhone</span><span class="sxs-lookup"><span data-stu-id="66b2d-126">-  MobilePhone</span></span>  <br/><span data-ttu-id="66b2d-127">-他の Fax</span><span class="sxs-lookup"><span data-stu-id="66b2d-127">-  OtherFax</span></span>  <br/><span data-ttu-id="66b2d-128">-他の電話</span><span class="sxs-lookup"><span data-stu-id="66b2d-128">-  OtherTelephone</span></span>  <br/><span data-ttu-id="66b2d-129">-ポケットベル</span><span class="sxs-lookup"><span data-stu-id="66b2d-129">-  Pager</span></span>  <br/><span data-ttu-id="66b2d-130">- PrimaryPhone</span><span class="sxs-lookup"><span data-stu-id="66b2d-130">-  PrimaryPhone</span></span>  <br/><span data-ttu-id="66b2d-131">- RadioPhone</span><span class="sxs-lookup"><span data-stu-id="66b2d-131">-  RadioPhone</span></span>  <br/><span data-ttu-id="66b2d-132">-テレックス</span><span class="sxs-lookup"><span data-stu-id="66b2d-132">-  Telex</span></span>  <br/><span data-ttu-id="66b2d-133">-TtyTddPhone</span><span class="sxs-lookup"><span data-stu-id="66b2d-133">-  TtyTddPhone</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="66b2d-134">子要素</span><span class="sxs-lookup"><span data-stu-id="66b2d-134">Child elements</span></span>

<span data-ttu-id="66b2d-135">なし。</span><span class="sxs-lookup"><span data-stu-id="66b2d-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="66b2d-136">親要素</span><span class="sxs-lookup"><span data-stu-id="66b2d-136">Parent elements</span></span>

|<span data-ttu-id="66b2d-137">**要素**</span><span class="sxs-lookup"><span data-stu-id="66b2d-137">**Element**</span></span>|<span data-ttu-id="66b2d-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="66b2d-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66b2d-139">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="66b2d-139">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="66b2d-140">連絡先の電話番号のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="66b2d-140">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="66b2d-141">テキスト値</span><span class="sxs-lookup"><span data-stu-id="66b2d-141">Text value</span></span>

<span data-ttu-id="66b2d-142">この要素を使用する場合は、電話番号を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="66b2d-142">A text value that represents a telephone number is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="66b2d-143">注釈</span><span class="sxs-lookup"><span data-stu-id="66b2d-143">Remarks</span></span>

<span data-ttu-id="66b2d-144">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="66b2d-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66b2d-145">要素の情報</span><span class="sxs-lookup"><span data-stu-id="66b2d-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66b2d-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="66b2d-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="66b2d-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="66b2d-147">Schema name</span></span>  <br/> |<span data-ttu-id="66b2d-148">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="66b2d-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="66b2d-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="66b2d-149">Validation file</span></span>  <br/> |<span data-ttu-id="66b2d-150">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="66b2d-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="66b2d-151">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="66b2d-151">Can be empty</span></span>  <br/> |<span data-ttu-id="66b2d-152">正しくない</span><span class="sxs-lookup"><span data-stu-id="66b2d-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66b2d-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="66b2d-153">See also</span></span>

- [<span data-ttu-id="66b2d-154">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="66b2d-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="66b2d-155">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="66b2d-155">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [<span data-ttu-id="66b2d-156">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="66b2d-156">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="66b2d-157">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="66b2d-157">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

