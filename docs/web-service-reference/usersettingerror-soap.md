---
title: UserSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: abb175c5-4f38-4dcc-81e3-b511686862eb
description: UserSettingError 要素は、ユーザー設定を取得しようとした結果として返されるエラーを表します。
ms.openlocfilehash: 886e0be0aa900ce3a00902c21cc115e866d0cd99
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839954"
---
# <a name="usersettingerror-soap"></a><span data-ttu-id="e5ff8-103">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5ff8-103">UserSettingError (SOAP)</span></span>

<span data-ttu-id="e5ff8-104">**UserSettingError**要素は、ユーザー設定を取得しようとした結果として返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="e5ff8-104">The **UserSettingError** element represents an error that is returned as a result of an attempt to get a user setting.</span></span> 
  
```XML
<UserSettingError>
    <ErrorCode/>
    <ErrorMessage/>
    <SettingName/>
</UserSettingError>
```

 <span data-ttu-id="e5ff8-105">**UserSettingError**</span><span class="sxs-lookup"><span data-stu-id="e5ff8-105">**UserSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e5ff8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e5ff8-106">Attributes and elements</span></span>

<span data-ttu-id="e5ff8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e5ff8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5ff8-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5ff8-108">Attributes</span></span>

<span data-ttu-id="e5ff8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e5ff8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5ff8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e5ff8-110">Child elements</span></span>

|<span data-ttu-id="e5ff8-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e5ff8-111">**Element**</span></span>|<span data-ttu-id="e5ff8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e5ff8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5ff8-113">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5ff8-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="e5ff8-114">自動検出サービスによって返されるエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="e5ff8-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="e5ff8-115">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5ff8-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="e5ff8-116">自動検出サービスによって返されるエラー コードに関連付けられているメッセージを示す。</span><span class="sxs-lookup"><span data-stu-id="e5ff8-116">Respresents a message associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="e5ff8-117">SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5ff8-117">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="e5ff8-118">ユーザー設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="e5ff8-118">Represents the name of a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e5ff8-119">親要素</span><span class="sxs-lookup"><span data-stu-id="e5ff8-119">Parent elements</span></span>

|<span data-ttu-id="e5ff8-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="e5ff8-120">**Element**</span></span>|<span data-ttu-id="e5ff8-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="e5ff8-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5ff8-122">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5ff8-122">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="e5ff8-123">返されませんでしたの設定に関する情報のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e5ff8-123">Represents a collection of information about settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e5ff8-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e5ff8-124">Text value</span></span>

<span data-ttu-id="e5ff8-125">なし。</span><span class="sxs-lookup"><span data-stu-id="e5ff8-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5ff8-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="e5ff8-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5ff8-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="e5ff8-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e5ff8-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e5ff8-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e5ff8-129">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="e5ff8-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e5ff8-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e5ff8-130">Validation File</span></span>  <br/> |<span data-ttu-id="e5ff8-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e5ff8-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e5ff8-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e5ff8-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e5ff8-133">True</span><span class="sxs-lookup"><span data-stu-id="e5ff8-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e5ff8-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="e5ff8-134">See also</span></span>



[<span data-ttu-id="e5ff8-135">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="e5ff8-135">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

