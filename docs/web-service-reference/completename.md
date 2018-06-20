---
title: CompleteName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteName
api_type:
- schema
ms.assetid: 22d30d1f-a84d-48bb-ad8f-ce13f8e76604
description: CompleteName 要素は、連絡先の完全な名前を表します。
ms.openlocfilehash: 1f6c9ba68fe941f848d0e250a39aea6894fca61e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759638"
---
# <a name="completename"></a><span data-ttu-id="1acd5-103">CompleteName</span><span class="sxs-lookup"><span data-stu-id="1acd5-103">CompleteName</span></span>

<span data-ttu-id="1acd5-104">**CompleteName**要素は、連絡先の完全な名前を表します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-104">The **CompleteName** element represents the complete name of a contact.</span></span> 
  
```xml
<CompleteName>
   <Title/>
   <FirstName/>
   <MiddleName/>
   <LastName/>
   <Suffix/>
   <Initials/>
   <FullName/>
   <Nickname/>
   <YomiFirstName/>
   <YomiLastName/>
</CompleteName>
```

 <span data-ttu-id="1acd5-105">**CompleteNameType**</span><span class="sxs-lookup"><span data-stu-id="1acd5-105">**CompleteNameType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1acd5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1acd5-106">Attributes and elements</span></span>

<span data-ttu-id="1acd5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1acd5-108">属性</span><span class="sxs-lookup"><span data-stu-id="1acd5-108">Attributes</span></span>

<span data-ttu-id="1acd5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1acd5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1acd5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1acd5-110">Child elements</span></span>

|<span data-ttu-id="1acd5-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1acd5-111">**Element**</span></span>|<span data-ttu-id="1acd5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1acd5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1acd5-113">Title</span><span class="sxs-lookup"><span data-stu-id="1acd5-113">Title</span></span>](title.md) <br/> |<span data-ttu-id="1acd5-114">連絡先のタイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-114">Represents the title of a contact.</span></span>  <br/> |
|<span data-ttu-id="1acd5-115">[[部署名]](firstname.md)</span><span class="sxs-lookup"><span data-stu-id="1acd5-115">[FirstName](firstname.md)</span></span> <br/> |<span data-ttu-id="1acd5-116">連絡先の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-116">Represents the first name of contact.</span></span>  <br/> |
|[<span data-ttu-id="1acd5-117">ミドル ネーム</span><span class="sxs-lookup"><span data-stu-id="1acd5-117">MiddleName</span></span>](middlename.md) <br/> |<span data-ttu-id="1acd5-118">連絡先のミドル ネームを表します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-118">Represents the middle name of a contact.</span></span>  <br/> |
|<span data-ttu-id="1acd5-119">[[氏名]](lastname.md)</span><span class="sxs-lookup"><span data-stu-id="1acd5-119">[LastName](lastname.md)</span></span> <br/> |<span data-ttu-id="1acd5-120">連絡先の姓を表します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-120">Represents the last name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="1acd5-121">Suffix</span><span class="sxs-lookup"><span data-stu-id="1acd5-121">Suffix</span></span>](suffix.md) <br/> |<span data-ttu-id="1acd5-122">連絡先の名前にサフィックスを表します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-122">Represents a suffix to a contact's name.</span></span>  <br/> |
|<span data-ttu-id="1acd5-123">[[頭文字]](initials.md)</span><span class="sxs-lookup"><span data-stu-id="1acd5-123">[Initials](initials.md)</span></span> <br/> |<span data-ttu-id="1acd5-124">連絡先のイニシャルを表します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-124">Represents the initials of a contact.</span></span>  <br/> |
|[<span data-ttu-id="1acd5-125">FullName</span><span class="sxs-lookup"><span data-stu-id="1acd5-125">FullName</span></span>](fullname.md) <br/> |<span data-ttu-id="1acd5-126">連絡先の完全名を表します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-126">Represents the full name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="1acd5-127">ニックネーム</span><span class="sxs-lookup"><span data-stu-id="1acd5-127">Nickname</span></span>](nickname.md) <br/> |<span data-ttu-id="1acd5-128">連絡先のニックネームを表します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-128">Represents the nickname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="1acd5-129">YomiFirstName</span><span class="sxs-lookup"><span data-stu-id="1acd5-129">YomiFirstName</span></span>](yomifirstname.md) <br/> |<span data-ttu-id="1acd5-130">日本語の姓の検索可能なまたはふりがなのスペル チェックを日本で使用される名前を表します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-130">Represents the name used in Japan for the searchable or phonetic spelling of a Japanese first name.</span></span>  <br/> |
|[<span data-ttu-id="1acd5-131">YomiLastName</span><span class="sxs-lookup"><span data-stu-id="1acd5-131">YomiLastName</span></span>](yomilastname.md) <br/> |<span data-ttu-id="1acd5-132">日本語の姓のふりがな、または検索可能なスペルの日本で使用される名前を表します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-132">Represents the name used in Japan for the searchable or phonetic spelling of a Japanese last name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1acd5-133">親要素</span><span class="sxs-lookup"><span data-stu-id="1acd5-133">Parent elements</span></span>

|<span data-ttu-id="1acd5-134">**要素**</span><span class="sxs-lookup"><span data-stu-id="1acd5-134">**Element**</span></span>|<span data-ttu-id="1acd5-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="1acd5-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1acd5-136">Contact</span><span class="sxs-lookup"><span data-stu-id="1acd5-136">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="1acd5-137">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-137">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1acd5-138">備考</span><span class="sxs-lookup"><span data-stu-id="1acd5-138">Remarks</span></span>

<span data-ttu-id="1acd5-139">[CompleteName](completename.md)プロパティは、[既定](https://msdn.microsoft.com/library/ExchangeWebServices.DefaultShapeNamesType.Default.aspx)の図形の一部です。</span><span class="sxs-lookup"><span data-stu-id="1acd5-139">The [CompleteName](completename.md) property is part of the [Default](https://msdn.microsoft.com/library/ExchangeWebServices.DefaultShapeNamesType.Default.aspx) shape.</span></span> <span data-ttu-id="1acd5-140">Microsoft Exchange Server 2007 の最初のリリース バージョン、 [GetItem 操作](getitem-operation.md)が[FindItem 操作](finditem-operation.md)ではなく、 [CompleteName](completename.md)プロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1acd5-140">In the initial release version of Microsoft Exchange Server 2007, the [CompleteName](completename.md) property is returned by the [GetItem operation](getitem-operation.md), but not the [FindItem operation](finditem-operation.md).</span></span> <span data-ttu-id="1acd5-141">Exchange Server 2007 Service Pack 1 (SP1) から始めて、 [FindItem 操作](finditem-operation.md)はまた、[既定](https://msdn.microsoft.com/library/ExchangeWebServices.DefaultShapeNamesType.Default.aspx)の図形を使用して[CompleteName](completename.md)プロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-141">Starting with Exchange Server 2007 Service Pack 1 (SP1), the [FindItem operation](finditem-operation.md) also returns the [CompleteName](completename.md) property with the [Default](https://msdn.microsoft.com/library/ExchangeWebServices.DefaultShapeNamesType.Default.aspx) shape.</span></span> <span data-ttu-id="1acd5-142">この変更は、スキーマには影響しません。</span><span class="sxs-lookup"><span data-stu-id="1acd5-142">This change does not affect the schema.</span></span> 
  
<span data-ttu-id="1acd5-143">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1acd5-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1acd5-144">要素情報</span><span class="sxs-lookup"><span data-stu-id="1acd5-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1acd5-145">名前空間</span><span class="sxs-lookup"><span data-stu-id="1acd5-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1acd5-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1acd5-146">Schema name</span></span>  <br/> |<span data-ttu-id="1acd5-147">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1acd5-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="1acd5-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1acd5-148">Validation file</span></span>  <br/> |<span data-ttu-id="1acd5-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1acd5-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1acd5-150">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1acd5-150">Can be empty</span></span>  <br/> |<span data-ttu-id="1acd5-151">False</span><span class="sxs-lookup"><span data-stu-id="1acd5-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1acd5-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="1acd5-152">See also</span></span>



[<span data-ttu-id="1acd5-153">CompleteNameType</span><span class="sxs-lookup"><span data-stu-id="1acd5-153">CompleteNameType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CompleteNameType.aspx)
  
[<span data-ttu-id="1acd5-154">CompleteName</span><span class="sxs-lookup"><span data-stu-id="1acd5-154">CompleteName</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ContactItemType.CompleteName.aspx)
  
[<span data-ttu-id="1acd5-155">contactsCompleteName</span><span class="sxs-lookup"><span data-stu-id="1acd5-155">contactsCompleteName</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.UnindexedFieldURIType.contactsCompleteName.aspx)


- [<span data-ttu-id="1acd5-156">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1acd5-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="1acd5-157">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="1acd5-157">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

