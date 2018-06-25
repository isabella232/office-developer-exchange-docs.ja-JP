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
ms.openlocfilehash: 43161e0adb4a98d354873e65868ddae37cd80e97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832773"
---
# <a name="phonenumbers"></a><span data-ttu-id="6c7cf-103">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="6c7cf-103">PhoneNumbers</span></span>

<span data-ttu-id="6c7cf-104">**PhoneNumbers**要素は、連絡先の電話番号のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="6c7cf-104">The **PhoneNumbers** element represents a collection of telephone numbers for a contact.</span></span> 
  
```xml
<PhoneNumbers>
   <Entry/>
</PhoneNumbers>
```

 <span data-ttu-id="6c7cf-105">**PhoneNumberDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="6c7cf-105">**PhoneNumberDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c7cf-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6c7cf-106">Attributes and elements</span></span>

<span data-ttu-id="6c7cf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c7cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c7cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="6c7cf-108">Attributes</span></span>

<span data-ttu-id="6c7cf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6c7cf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c7cf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6c7cf-110">Child elements</span></span>

|<span data-ttu-id="6c7cf-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c7cf-111">**Element**</span></span>|<span data-ttu-id="6c7cf-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c7cf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c7cf-113">入力 (電話番号)</span><span class="sxs-lookup"><span data-stu-id="6c7cf-113">Entry (PhoneNumber)</span></span>](entry-phonenumber.md) <br/> |<span data-ttu-id="6c7cf-114">連絡先の電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="6c7cf-114">Represents a telephone number for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6c7cf-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6c7cf-115">Parent elements</span></span>

|<span data-ttu-id="6c7cf-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c7cf-116">**Element**</span></span>|<span data-ttu-id="6c7cf-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c7cf-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c7cf-118">Contact</span><span class="sxs-lookup"><span data-stu-id="6c7cf-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="6c7cf-119">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6c7cf-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6c7cf-120">備考</span><span class="sxs-lookup"><span data-stu-id="6c7cf-120">Remarks</span></span>

<span data-ttu-id="6c7cf-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="6c7cf-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c7cf-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="6c7cf-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c7cf-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="6c7cf-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6c7cf-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c7cf-124">Schema name</span></span>  <br/> |<span data-ttu-id="6c7cf-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6c7cf-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="6c7cf-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c7cf-126">Validation file</span></span>  <br/> |<span data-ttu-id="6c7cf-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6c7cf-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6c7cf-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6c7cf-128">Can be empty</span></span>  <br/> |<span data-ttu-id="6c7cf-129">False</span><span class="sxs-lookup"><span data-stu-id="6c7cf-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c7cf-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c7cf-130">See also</span></span>



- [<span data-ttu-id="6c7cf-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6c7cf-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6c7cf-132">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="6c7cf-132">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="6c7cf-133">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="6c7cf-133">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="6c7cf-134">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="6c7cf-134">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

