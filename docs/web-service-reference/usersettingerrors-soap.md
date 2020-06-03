---
title: UserSettingErrors (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a9b94bae-cab9-412d-a811-801e849ed6c5
description: UserSettingErrors 要素は、返すことができなかった設定に関する情報のコレクションを表します。
ms.openlocfilehash: a6cc0fe114bd511dc4136532986b552c28b0d5c2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467124"
---
# <a name="usersettingerrors-soap"></a><span data-ttu-id="dae06-103">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dae06-103">UserSettingErrors (SOAP)</span></span>

<span data-ttu-id="dae06-104">**Usersettingerrors**要素は、返すことができなかった設定に関する情報のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="dae06-104">The **UserSettingErrors** element represents a collection of information about settings that could not be returned.</span></span> 
  
```XML
<UserSettingErrors>
    <UserSettingError/>
</UserSettingErrors>
```

 <span data-ttu-id="dae06-105">**UserSettingErrors**</span><span class="sxs-lookup"><span data-stu-id="dae06-105">**UserSettingErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dae06-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dae06-106">Attributes and elements</span></span>

<span data-ttu-id="dae06-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dae06-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dae06-108">属性</span><span class="sxs-lookup"><span data-stu-id="dae06-108">Attributes</span></span>

<span data-ttu-id="dae06-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dae06-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dae06-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dae06-110">Child elements</span></span>

|<span data-ttu-id="dae06-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="dae06-111">**Element**</span></span>|<span data-ttu-id="dae06-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dae06-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dae06-113">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dae06-113">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="dae06-114">ユーザー設定の取得中に返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="dae06-114">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dae06-115">親要素</span><span class="sxs-lookup"><span data-stu-id="dae06-115">Parent elements</span></span>

|<span data-ttu-id="dae06-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="dae06-116">**Element**</span></span>|<span data-ttu-id="dae06-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="dae06-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dae06-118">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dae06-118">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="dae06-119">個々のユーザーに対する GetUserSettings 要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="dae06-119">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dae06-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dae06-120">Text value</span></span>

<span data-ttu-id="dae06-121">なし。</span><span class="sxs-lookup"><span data-stu-id="dae06-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dae06-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dae06-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dae06-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="dae06-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="dae06-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dae06-124">Schema Name</span></span>  <br/> |<span data-ttu-id="dae06-125">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="dae06-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="dae06-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dae06-126">Validation File</span></span>  <br/> |<span data-ttu-id="dae06-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="dae06-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dae06-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dae06-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="dae06-129">正しい</span><span class="sxs-lookup"><span data-stu-id="dae06-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dae06-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="dae06-130">See also</span></span>



[<span data-ttu-id="dae06-131">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="dae06-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

