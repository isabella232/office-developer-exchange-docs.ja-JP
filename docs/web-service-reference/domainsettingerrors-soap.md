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
description: DomainSettingsErrors 要素には、返されなかった設定に関するエラー情報が含まれています。
ms.openlocfilehash: 4e7ee29c2bc680a1938b75189c2ac3c214f7d2b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530706"
---
# <a name="domainsettingerrors-soap"></a><span data-ttu-id="eb5d7-103">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb5d7-103">DomainSettingErrors (SOAP)</span></span>

<span data-ttu-id="eb5d7-104">**DomainSettingsErrors**要素には、返されなかった設定に関するエラー情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb5d7-104">The **DomainSettingsErrors** element contains error information for settings that could not be returned.</span></span> 
  
```XML
<DomainSettingsErrors>
   <DomainSettingsError/>
</DomainSettingsErrors>
```

 <span data-ttu-id="eb5d7-105">**DomainSettingsErrors**</span><span class="sxs-lookup"><span data-stu-id="eb5d7-105">**DomainSettingsErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb5d7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="eb5d7-106">Attributes and elements</span></span>

<span data-ttu-id="eb5d7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eb5d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb5d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="eb5d7-108">Attributes</span></span>

<span data-ttu-id="eb5d7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="eb5d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb5d7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="eb5d7-110">Child elements</span></span>

|<span data-ttu-id="eb5d7-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="eb5d7-111">**Element**</span></span>|<span data-ttu-id="eb5d7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb5d7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb5d7-113">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb5d7-113">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="eb5d7-114">ドメイン設定の取得中に発生したエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="eb5d7-114">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="eb5d7-115">これは、 [Getdomainsettings 操作 (SOAP)](getdomainsettings-operation-soap.md)操作要求からのエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="eb5d7-115">This represents an error from a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb5d7-116">親要素</span><span class="sxs-lookup"><span data-stu-id="eb5d7-116">Parent elements</span></span>

|<span data-ttu-id="eb5d7-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="eb5d7-117">**Element**</span></span>|<span data-ttu-id="eb5d7-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb5d7-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb5d7-119">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb5d7-119">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="eb5d7-120">指定したドメインに対して要求された設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="eb5d7-120">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eb5d7-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="eb5d7-121">Text value</span></span>

<span data-ttu-id="eb5d7-122">なし。</span><span class="sxs-lookup"><span data-stu-id="eb5d7-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb5d7-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="eb5d7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb5d7-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="eb5d7-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="eb5d7-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eb5d7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="eb5d7-126">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="eb5d7-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="eb5d7-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eb5d7-127">Validation File</span></span>  <br/> |<span data-ttu-id="eb5d7-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="eb5d7-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eb5d7-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="eb5d7-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb5d7-130">正しい</span><span class="sxs-lookup"><span data-stu-id="eb5d7-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb5d7-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="eb5d7-131">See also</span></span>

- [<span data-ttu-id="eb5d7-132">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb5d7-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

