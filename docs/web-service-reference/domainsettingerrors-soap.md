---
title: DomainSettingErrors (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a4ce19de-f560-4984-8047-ecbbc86c9b91
description: DomainSettingsErrors 要素には、エラーは返されませんでしたの設定情報が含まれています。
ms.openlocfilehash: 6ecd23bc556ca32d724581a28cc7c117c6853207
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760165"
---
# <a name="domainsettingerrors-soap"></a><span data-ttu-id="49637-103">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="49637-103">DomainSettingErrors (SOAP)</span></span>

<span data-ttu-id="49637-104">**DomainSettingsErrors**要素には、エラーは返されませんでしたの設定情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="49637-104">The **DomainSettingsErrors** element contains error information for settings that could not be returned.</span></span> 
  
```XML
<DomainSettingsErrors>
   <DomainSettingsError/>
</DomainSettingsErrors>
```

 <span data-ttu-id="49637-105">**DomainSettingsErrors**</span><span class="sxs-lookup"><span data-stu-id="49637-105">**DomainSettingsErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49637-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="49637-106">Attributes and elements</span></span>

<span data-ttu-id="49637-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="49637-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49637-108">属性</span><span class="sxs-lookup"><span data-stu-id="49637-108">Attributes</span></span>

<span data-ttu-id="49637-109">なし。</span><span class="sxs-lookup"><span data-stu-id="49637-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49637-110">子要素</span><span class="sxs-lookup"><span data-stu-id="49637-110">Child elements</span></span>

|<span data-ttu-id="49637-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="49637-111">**Element**</span></span>|<span data-ttu-id="49637-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="49637-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49637-113">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="49637-113">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="49637-114">ドメインの設定を取得中に発生したエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="49637-114">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="49637-115">これは、 [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)操作要求のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="49637-115">This represents an error from a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49637-116">親要素</span><span class="sxs-lookup"><span data-stu-id="49637-116">Parent elements</span></span>

|<span data-ttu-id="49637-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="49637-117">**Element**</span></span>|<span data-ttu-id="49637-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="49637-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49637-119">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="49637-119">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="49637-120">指定したドメインの指定された設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="49637-120">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="49637-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="49637-121">Text value</span></span>

<span data-ttu-id="49637-122">なし。</span><span class="sxs-lookup"><span data-stu-id="49637-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49637-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="49637-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49637-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="49637-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="49637-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="49637-125">Schema Name</span></span>  <br/> |<span data-ttu-id="49637-126">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="49637-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="49637-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="49637-127">Validation File</span></span>  <br/> |<span data-ttu-id="49637-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="49637-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="49637-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="49637-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="49637-130">True</span><span class="sxs-lookup"><span data-stu-id="49637-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49637-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="49637-131">See also</span></span>

- [<span data-ttu-id="49637-132">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="49637-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

