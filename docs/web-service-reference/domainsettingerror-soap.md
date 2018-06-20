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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760158"
---
# <a name="domainsettingerror-soap"></a><span data-ttu-id="ab4ee-104">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ab4ee-104">DomainSettingError (SOAP)</span></span>

<span data-ttu-id="ab4ee-105">**DomainSettingError**要素は、ドメインの設定を取得中に発生したエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="ab4ee-105">The **DomainSettingError** element represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="ab4ee-106">これは、 **GetDomainSettings**要求のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="ab4ee-106">This represents an error from a **GetDomainSettings** request.</span></span> 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 <span data-ttu-id="ab4ee-107">**DomainSettingError**</span><span class="sxs-lookup"><span data-stu-id="ab4ee-107">**DomainSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ab4ee-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ab4ee-108">Attributes and elements</span></span>

<span data-ttu-id="ab4ee-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ab4ee-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ab4ee-110">属性</span><span class="sxs-lookup"><span data-stu-id="ab4ee-110">Attributes</span></span>

<span data-ttu-id="ab4ee-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ab4ee-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ab4ee-112">子要素</span><span class="sxs-lookup"><span data-stu-id="ab4ee-112">Child elements</span></span>

|<span data-ttu-id="ab4ee-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ab4ee-113">**Element**</span></span>|<span data-ttu-id="ab4ee-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ab4ee-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ab4ee-115">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ab4ee-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="ab4ee-116">特定の要求に関連付けられているエラー コードを識別します。</span><span class="sxs-lookup"><span data-stu-id="ab4ee-116">Identifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="ab4ee-117">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ab4ee-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="ab4ee-118">特定の要求に関連付けられているエラー メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ab4ee-118">Contains the error message that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="ab4ee-119">SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ab4ee-119">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="ab4ee-120">設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="ab4ee-120">Represents the name of the setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ab4ee-121">親要素</span><span class="sxs-lookup"><span data-stu-id="ab4ee-121">Parent elements</span></span>

|<span data-ttu-id="ab4ee-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="ab4ee-122">**Element**</span></span>|<span data-ttu-id="ab4ee-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="ab4ee-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ab4ee-124">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ab4ee-124">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="ab4ee-125">返されませんでしたの設定に関するエラー情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ab4ee-125">Contains error information for settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ab4ee-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ab4ee-126">Text value</span></span>

<span data-ttu-id="ab4ee-127">なし。</span><span class="sxs-lookup"><span data-stu-id="ab4ee-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ab4ee-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="ab4ee-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ab4ee-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="ab4ee-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ab4ee-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ab4ee-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ab4ee-131">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="ab4ee-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ab4ee-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ab4ee-132">Validation File</span></span>  <br/> |<span data-ttu-id="ab4ee-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ab4ee-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ab4ee-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ab4ee-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ab4ee-135">True</span><span class="sxs-lookup"><span data-stu-id="ab4ee-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ab4ee-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="ab4ee-136">See also</span></span>

- [<span data-ttu-id="ab4ee-137">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ab4ee-137">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

