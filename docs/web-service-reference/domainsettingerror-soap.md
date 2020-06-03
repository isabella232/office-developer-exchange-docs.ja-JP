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
description: DomainSettingError 要素は、ドメイン設定の取得中に発生したエラーを表します。 これは、GetDomainSettings 要求からのエラーを表します。
ms.openlocfilehash: 189a614e7629033c8db2f60b8fd3679835a696ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530713"
---
# <a name="domainsettingerror-soap"></a><span data-ttu-id="d8b82-104">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d8b82-104">DomainSettingError (SOAP)</span></span>

<span data-ttu-id="d8b82-105">**Domainsettingerror**要素は、ドメイン設定の取得中に発生したエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="d8b82-105">The **DomainSettingError** element represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="d8b82-106">これは、 **Getdomainsettings**要求からのエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="d8b82-106">This represents an error from a **GetDomainSettings** request.</span></span> 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 <span data-ttu-id="d8b82-107">**DomainSettingError**</span><span class="sxs-lookup"><span data-stu-id="d8b82-107">**DomainSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8b82-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d8b82-108">Attributes and elements</span></span>

<span data-ttu-id="d8b82-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d8b82-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8b82-110">属性</span><span class="sxs-lookup"><span data-stu-id="d8b82-110">Attributes</span></span>

<span data-ttu-id="d8b82-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d8b82-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8b82-112">子要素</span><span class="sxs-lookup"><span data-stu-id="d8b82-112">Child elements</span></span>

|<span data-ttu-id="d8b82-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="d8b82-113">**Element**</span></span>|<span data-ttu-id="d8b82-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d8b82-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8b82-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d8b82-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="d8b82-116">特定の要求に関連付けられているエラーコードを識別します。</span><span class="sxs-lookup"><span data-stu-id="d8b82-116">Identifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="d8b82-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d8b82-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="d8b82-118">特定の要求に関連付けられているエラーメッセージが保存されています。</span><span class="sxs-lookup"><span data-stu-id="d8b82-118">Contains the error message that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="d8b82-119">SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d8b82-119">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="d8b82-120">設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="d8b82-120">Represents the name of the setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8b82-121">親要素</span><span class="sxs-lookup"><span data-stu-id="d8b82-121">Parent elements</span></span>

|<span data-ttu-id="d8b82-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="d8b82-122">**Element**</span></span>|<span data-ttu-id="d8b82-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="d8b82-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8b82-124">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d8b82-124">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="d8b82-125">返すことができなかった設定に関するエラー情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d8b82-125">Contains error information for settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d8b82-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d8b82-126">Text value</span></span>

<span data-ttu-id="d8b82-127">なし。</span><span class="sxs-lookup"><span data-stu-id="d8b82-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8b82-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d8b82-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8b82-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="d8b82-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d8b82-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d8b82-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d8b82-131">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="d8b82-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d8b82-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d8b82-132">Validation File</span></span>  <br/> |<span data-ttu-id="d8b82-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d8b82-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d8b82-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d8b82-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8b82-135">正しい</span><span class="sxs-lookup"><span data-stu-id="d8b82-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8b82-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="d8b82-136">See also</span></span>

- [<span data-ttu-id="d8b82-137">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d8b82-137">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

