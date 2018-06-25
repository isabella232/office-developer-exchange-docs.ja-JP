---
title: DomainSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 48c3f7b5-2ee0-42ce-97a1-a881e2f60327
description: DomainSettingError 要素は、ドメインの設定を取得中に発生したエラーを表します。 これは、GetDomainSettings 要求のエラーを表します。
ms.openlocfilehash: 08b0a47acea8d35ec78efd701168a251771effac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760158"
---
# <a name="domainsettingerror-soap"></a><span data-ttu-id="45e0a-104">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="45e0a-104">DomainSettingError (SOAP)</span></span>

<span data-ttu-id="45e0a-105">**DomainSettingError**要素は、ドメインの設定を取得中に発生したエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="45e0a-105">The **DomainSettingError** element represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="45e0a-106">これは、 **GetDomainSettings**要求のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="45e0a-106">This represents an error from a **GetDomainSettings** request.</span></span> 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 <span data-ttu-id="45e0a-107">**DomainSettingError**</span><span class="sxs-lookup"><span data-stu-id="45e0a-107">**DomainSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45e0a-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="45e0a-108">Attributes and elements</span></span>

<span data-ttu-id="45e0a-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="45e0a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45e0a-110">属性</span><span class="sxs-lookup"><span data-stu-id="45e0a-110">Attributes</span></span>

<span data-ttu-id="45e0a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="45e0a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="45e0a-112">子要素</span><span class="sxs-lookup"><span data-stu-id="45e0a-112">Child elements</span></span>

|<span data-ttu-id="45e0a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="45e0a-113">**Element**</span></span>|<span data-ttu-id="45e0a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="45e0a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45e0a-115">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="45e0a-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="45e0a-116">特定の要求に関連付けられているエラー コードを識別します。</span><span class="sxs-lookup"><span data-stu-id="45e0a-116">Identifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="45e0a-117">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="45e0a-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="45e0a-118">特定の要求に関連付けられているエラー メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="45e0a-118">Contains the error message that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="45e0a-119">SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="45e0a-119">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="45e0a-120">設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="45e0a-120">Represents the name of the setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="45e0a-121">親要素</span><span class="sxs-lookup"><span data-stu-id="45e0a-121">Parent elements</span></span>

|<span data-ttu-id="45e0a-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="45e0a-122">**Element**</span></span>|<span data-ttu-id="45e0a-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="45e0a-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45e0a-124">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="45e0a-124">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="45e0a-125">返されませんでしたの設定に関するエラー情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="45e0a-125">Contains error information for settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="45e0a-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="45e0a-126">Text value</span></span>

<span data-ttu-id="45e0a-127">なし。</span><span class="sxs-lookup"><span data-stu-id="45e0a-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45e0a-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="45e0a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45e0a-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="45e0a-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="45e0a-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="45e0a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="45e0a-131">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="45e0a-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="45e0a-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="45e0a-132">Validation File</span></span>  <br/> |<span data-ttu-id="45e0a-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="45e0a-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="45e0a-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="45e0a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="45e0a-135">True</span><span class="sxs-lookup"><span data-stu-id="45e0a-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="45e0a-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="45e0a-136">See also</span></span>

- [<span data-ttu-id="45e0a-137">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="45e0a-137">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

