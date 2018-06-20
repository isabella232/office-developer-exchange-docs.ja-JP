---
title: 入力 (電話番号)
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
description: エントリ要素は、連絡先の電話番号を表します。
ms.openlocfilehash: 3953488fb0b57fcf01c2fb99039478bbe03c7f5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760317"
---
# <a name="entry-phonenumber"></a><span data-ttu-id="feda6-103">入力 (電話番号)</span><span class="sxs-lookup"><span data-stu-id="feda6-103">Entry (PhoneNumber)</span></span>

<span data-ttu-id="feda6-104">**エントリ**要素は、連絡先の電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="feda6-104">The **Entry** element represents a telephone number for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="feda6-105">**PhoneNumberDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="feda6-105">**PhoneNumberDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="feda6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="feda6-106">Attributes and elements</span></span>

<span data-ttu-id="feda6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="feda6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="feda6-108">属性</span><span class="sxs-lookup"><span data-stu-id="feda6-108">Attributes</span></span>

|<span data-ttu-id="feda6-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="feda6-109">**Attribute**</span></span>|<span data-ttu-id="feda6-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="feda6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="feda6-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="feda6-111">**Key**</span></span> <br/> | <span data-ttu-id="feda6-112">電話番号を識別します。</span><span class="sxs-lookup"><span data-stu-id="feda6-112">Identifies the telephone number.</span></span> <span data-ttu-id="feda6-113">Key 属性は、型**PhoneNumberKeyType**のです。</span><span class="sxs-lookup"><span data-stu-id="feda6-113">The Key attribute is of type **PhoneNumberKeyType**.</span></span><br/><br/> <span data-ttu-id="feda6-114">次に、この属性で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="feda6-114">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="feda6-115">-AssistantPhone</span><span class="sxs-lookup"><span data-stu-id="feda6-115">-  AssistantPhone</span></span>  <br/><span data-ttu-id="feda6-116">-BusinessFax</span><span class="sxs-lookup"><span data-stu-id="feda6-116">-  BusinessFax</span></span>  <br/><span data-ttu-id="feda6-117">-BusinessPhone</span><span class="sxs-lookup"><span data-stu-id="feda6-117">-  BusinessPhone</span></span>  <br/><span data-ttu-id="feda6-118">-BusinessPhone2</span><span class="sxs-lookup"><span data-stu-id="feda6-118">-  BusinessPhone2</span></span>  <br/><span data-ttu-id="feda6-119">コールバック</span><span class="sxs-lookup"><span data-stu-id="feda6-119">-  Callback</span></span>  <br/><span data-ttu-id="feda6-120">-CarPhone</span><span class="sxs-lookup"><span data-stu-id="feda6-120">-  CarPhone</span></span>  <br/><span data-ttu-id="feda6-121">-CompanyMainPhone</span><span class="sxs-lookup"><span data-stu-id="feda6-121">-  CompanyMainPhone</span></span>  <br/><span data-ttu-id="feda6-122">-HomeFax</span><span class="sxs-lookup"><span data-stu-id="feda6-122">-  HomeFax</span></span>  <br/><span data-ttu-id="feda6-123">-HomePhone</span><span class="sxs-lookup"><span data-stu-id="feda6-123">-  HomePhone</span></span>  <br/><span data-ttu-id="feda6-124">-HomePhone2</span><span class="sxs-lookup"><span data-stu-id="feda6-124">-  HomePhone2</span></span>  <br/><span data-ttu-id="feda6-125">Isdn</span><span class="sxs-lookup"><span data-stu-id="feda6-125">-  Isdn</span></span>  <br/><span data-ttu-id="feda6-126">-MobilePhone</span><span class="sxs-lookup"><span data-stu-id="feda6-126">-  MobilePhone</span></span>  <br/><span data-ttu-id="feda6-127">-OtherFax</span><span class="sxs-lookup"><span data-stu-id="feda6-127">-  OtherFax</span></span>  <br/><span data-ttu-id="feda6-128">-OtherTelephone</span><span class="sxs-lookup"><span data-stu-id="feda6-128">-  OtherTelephone</span></span>  <br/><span data-ttu-id="feda6-129">ページ</span><span class="sxs-lookup"><span data-stu-id="feda6-129">-  Pager</span></span>  <br/><span data-ttu-id="feda6-130">-PrimaryPhone</span><span class="sxs-lookup"><span data-stu-id="feda6-130">-  PrimaryPhone</span></span>  <br/><span data-ttu-id="feda6-131">-RadioPhone</span><span class="sxs-lookup"><span data-stu-id="feda6-131">-  RadioPhone</span></span>  <br/><span data-ttu-id="feda6-132">-[テレックス</span><span class="sxs-lookup"><span data-stu-id="feda6-132">-  Telex</span></span>  <br/><span data-ttu-id="feda6-133">-TtyTddPhone</span><span class="sxs-lookup"><span data-stu-id="feda6-133">-  TtyTddPhone</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="feda6-134">子要素</span><span class="sxs-lookup"><span data-stu-id="feda6-134">Child elements</span></span>

<span data-ttu-id="feda6-135">なし。</span><span class="sxs-lookup"><span data-stu-id="feda6-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="feda6-136">親要素</span><span class="sxs-lookup"><span data-stu-id="feda6-136">Parent elements</span></span>

|<span data-ttu-id="feda6-137">**要素**</span><span class="sxs-lookup"><span data-stu-id="feda6-137">**Element**</span></span>|<span data-ttu-id="feda6-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="feda6-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="feda6-139">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="feda6-139">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="feda6-140">連絡先の電話番号のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="feda6-140">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="feda6-141">テキスト値</span><span class="sxs-lookup"><span data-stu-id="feda6-141">Text value</span></span>

<span data-ttu-id="feda6-142">電話番号を表す文字列値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="feda6-142">A text value that represents a telephone number is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="feda6-143">備考</span><span class="sxs-lookup"><span data-stu-id="feda6-143">Remarks</span></span>

<span data-ttu-id="feda6-144">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="feda6-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="feda6-145">要素情報</span><span class="sxs-lookup"><span data-stu-id="feda6-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="feda6-146">名前空間</span><span class="sxs-lookup"><span data-stu-id="feda6-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="feda6-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="feda6-147">Schema name</span></span>  <br/> |<span data-ttu-id="feda6-148">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="feda6-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="feda6-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="feda6-149">Validation file</span></span>  <br/> |<span data-ttu-id="feda6-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="feda6-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="feda6-151">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="feda6-151">Can be empty</span></span>  <br/> |<span data-ttu-id="feda6-152">False</span><span class="sxs-lookup"><span data-stu-id="feda6-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="feda6-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="feda6-153">See also</span></span>

- [<span data-ttu-id="feda6-154">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="feda6-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="feda6-155">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="feda6-155">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [<span data-ttu-id="feda6-156">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="feda6-156">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="feda6-157">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="feda6-157">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

