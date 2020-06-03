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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459638"
---
# <a name="entry-phonenumber"></a><span data-ttu-id="a6d47-103">Entry (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="a6d47-103">Entry (PhoneNumber)</span></span>

<span data-ttu-id="a6d47-104">**Entry**要素は、連絡先の電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="a6d47-104">The **Entry** element represents a telephone number for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="a6d47-105">**PhoneNumberDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="a6d47-105">**PhoneNumberDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a6d47-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a6d47-106">Attributes and elements</span></span>

<span data-ttu-id="a6d47-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a6d47-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6d47-108">属性</span><span class="sxs-lookup"><span data-stu-id="a6d47-108">Attributes</span></span>

|<span data-ttu-id="a6d47-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="a6d47-109">**Attribute**</span></span>|<span data-ttu-id="a6d47-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="a6d47-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a6d47-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="a6d47-111">**Key**</span></span> <br/> | <span data-ttu-id="a6d47-112">電話番号を識別します。</span><span class="sxs-lookup"><span data-stu-id="a6d47-112">Identifies the telephone number.</span></span> <span data-ttu-id="a6d47-113">キー属性の型は**PhoneNumberKeyType**です。</span><span class="sxs-lookup"><span data-stu-id="a6d47-113">The Key attribute is of type **PhoneNumberKeyType**.</span></span><br/><br/> <span data-ttu-id="a6d47-114">次に、この属性で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="a6d47-114">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="a6d47-115">- AssistantPhone</span><span class="sxs-lookup"><span data-stu-id="a6d47-115">-  AssistantPhone</span></span>  <br/><span data-ttu-id="a6d47-116">-BusinessFax</span><span class="sxs-lookup"><span data-stu-id="a6d47-116">-  BusinessFax</span></span>  <br/><span data-ttu-id="a6d47-117">- BusinessPhone</span><span class="sxs-lookup"><span data-stu-id="a6d47-117">-  BusinessPhone</span></span>  <br/><span data-ttu-id="a6d47-118">- BusinessPhone2</span><span class="sxs-lookup"><span data-stu-id="a6d47-118">-  BusinessPhone2</span></span>  <br/><span data-ttu-id="a6d47-119">-コールバック</span><span class="sxs-lookup"><span data-stu-id="a6d47-119">-  Callback</span></span>  <br/><span data-ttu-id="a6d47-120">-CarPhone</span><span class="sxs-lookup"><span data-stu-id="a6d47-120">-  CarPhone</span></span>  <br/><span data-ttu-id="a6d47-121">-会社の Mainphone</span><span class="sxs-lookup"><span data-stu-id="a6d47-121">-  CompanyMainPhone</span></span>  <br/><span data-ttu-id="a6d47-122">-ホーム Fax</span><span class="sxs-lookup"><span data-stu-id="a6d47-122">-  HomeFax</span></span>  <br/><span data-ttu-id="a6d47-123">-HomePhone</span><span class="sxs-lookup"><span data-stu-id="a6d47-123">-  HomePhone</span></span>  <br/><span data-ttu-id="a6d47-124">- HomePhone2</span><span class="sxs-lookup"><span data-stu-id="a6d47-124">-  HomePhone2</span></span>  <br/><span data-ttu-id="a6d47-125">-Isdn</span><span class="sxs-lookup"><span data-stu-id="a6d47-125">-  Isdn</span></span>  <br/><span data-ttu-id="a6d47-126">-MobilePhone</span><span class="sxs-lookup"><span data-stu-id="a6d47-126">-  MobilePhone</span></span>  <br/><span data-ttu-id="a6d47-127">-他の Fax</span><span class="sxs-lookup"><span data-stu-id="a6d47-127">-  OtherFax</span></span>  <br/><span data-ttu-id="a6d47-128">-他の電話</span><span class="sxs-lookup"><span data-stu-id="a6d47-128">-  OtherTelephone</span></span>  <br/><span data-ttu-id="a6d47-129">-ポケットベル</span><span class="sxs-lookup"><span data-stu-id="a6d47-129">-  Pager</span></span>  <br/><span data-ttu-id="a6d47-130">- PrimaryPhone</span><span class="sxs-lookup"><span data-stu-id="a6d47-130">-  PrimaryPhone</span></span>  <br/><span data-ttu-id="a6d47-131">- RadioPhone</span><span class="sxs-lookup"><span data-stu-id="a6d47-131">-  RadioPhone</span></span>  <br/><span data-ttu-id="a6d47-132">-テレックス</span><span class="sxs-lookup"><span data-stu-id="a6d47-132">-  Telex</span></span>  <br/><span data-ttu-id="a6d47-133">-TtyTddPhone</span><span class="sxs-lookup"><span data-stu-id="a6d47-133">-  TtyTddPhone</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a6d47-134">子要素</span><span class="sxs-lookup"><span data-stu-id="a6d47-134">Child elements</span></span>

<span data-ttu-id="a6d47-135">なし。</span><span class="sxs-lookup"><span data-stu-id="a6d47-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a6d47-136">親要素</span><span class="sxs-lookup"><span data-stu-id="a6d47-136">Parent elements</span></span>

|<span data-ttu-id="a6d47-137">**要素**</span><span class="sxs-lookup"><span data-stu-id="a6d47-137">**Element**</span></span>|<span data-ttu-id="a6d47-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="a6d47-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6d47-139">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="a6d47-139">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="a6d47-140">連絡先の電話番号のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a6d47-140">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a6d47-141">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a6d47-141">Text value</span></span>

<span data-ttu-id="a6d47-142">この要素を使用する場合は、電話番号を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6d47-142">A text value that represents a telephone number is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a6d47-143">注釈</span><span class="sxs-lookup"><span data-stu-id="a6d47-143">Remarks</span></span>

<span data-ttu-id="a6d47-144">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a6d47-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6d47-145">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a6d47-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6d47-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="a6d47-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a6d47-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a6d47-147">Schema name</span></span>  <br/> |<span data-ttu-id="a6d47-148">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a6d47-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="a6d47-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a6d47-149">Validation file</span></span>  <br/> |<span data-ttu-id="a6d47-150">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a6d47-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a6d47-151">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a6d47-151">Can be empty</span></span>  <br/> |<span data-ttu-id="a6d47-152">正しくない</span><span class="sxs-lookup"><span data-stu-id="a6d47-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a6d47-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="a6d47-153">See also</span></span>

- [<span data-ttu-id="a6d47-154">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a6d47-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="a6d47-155">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="a6d47-155">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [<span data-ttu-id="a6d47-156">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="a6d47-156">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="a6d47-157">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="a6d47-157">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

