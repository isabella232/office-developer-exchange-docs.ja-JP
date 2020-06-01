---
title: PhoneNumbers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneNumbers
api_type:
- schema
ms.assetid: 6cb71be1-c4fe-4ce7-9604-11fc01956ee9
description: PhoneNumbers 要素は、連絡先の電話番号のコレクションを表します。
ms.openlocfilehash: b64d811618176377048d9ba80d8d7573f2df034a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44440233"
---
# <a name="phonenumbers"></a><span data-ttu-id="31e16-103">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="31e16-103">PhoneNumbers</span></span>

<span data-ttu-id="31e16-104">**PhoneNumbers**要素は、連絡先の電話番号のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="31e16-104">The **PhoneNumbers** element represents a collection of telephone numbers for a contact.</span></span> 
  
```xml
<PhoneNumbers>
   <Entry/>
</PhoneNumbers>
```

 <span data-ttu-id="31e16-105">**PhoneNumberDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="31e16-105">**PhoneNumberDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31e16-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="31e16-106">Attributes and elements</span></span>

<span data-ttu-id="31e16-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="31e16-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31e16-108">属性</span><span class="sxs-lookup"><span data-stu-id="31e16-108">Attributes</span></span>

<span data-ttu-id="31e16-109">なし。</span><span class="sxs-lookup"><span data-stu-id="31e16-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31e16-110">子要素</span><span class="sxs-lookup"><span data-stu-id="31e16-110">Child elements</span></span>

|<span data-ttu-id="31e16-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="31e16-111">**Element**</span></span>|<span data-ttu-id="31e16-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="31e16-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31e16-113">Entry (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="31e16-113">Entry (PhoneNumber)</span></span>](entry-phonenumber.md) <br/> |<span data-ttu-id="31e16-114">連絡先の電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="31e16-114">Represents a telephone number for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="31e16-115">親要素</span><span class="sxs-lookup"><span data-stu-id="31e16-115">Parent elements</span></span>

|<span data-ttu-id="31e16-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="31e16-116">**Element**</span></span>|<span data-ttu-id="31e16-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="31e16-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31e16-118">連絡先</span><span class="sxs-lookup"><span data-stu-id="31e16-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="31e16-119">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="31e16-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="31e16-120">注釈</span><span class="sxs-lookup"><span data-stu-id="31e16-120">Remarks</span></span>

<span data-ttu-id="31e16-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="31e16-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31e16-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="31e16-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31e16-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="31e16-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="31e16-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="31e16-124">Schema name</span></span>  <br/> |<span data-ttu-id="31e16-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="31e16-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="31e16-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="31e16-126">Validation file</span></span>  <br/> |<span data-ttu-id="31e16-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="31e16-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="31e16-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="31e16-128">Can be empty</span></span>  <br/> |<span data-ttu-id="31e16-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="31e16-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31e16-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="31e16-130">See also</span></span>



- [<span data-ttu-id="31e16-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="31e16-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="31e16-132">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="31e16-132">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="31e16-133">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="31e16-133">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="31e16-134">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="31e16-134">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

