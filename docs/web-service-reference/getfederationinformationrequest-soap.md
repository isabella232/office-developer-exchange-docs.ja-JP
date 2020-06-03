---
title: GetFederationInformationRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: df5bface-f070-49e0-8527-6129ed8e8095
description: GetFederationInformationRequest 要素は、GetFederationInformation 操作 (SOAP) 操作の呼び出しのパラメーターを表します。
ms.openlocfilehash: 1df0a88ed8fbc75eb5723d1390baeefd3ad73652
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456585"
---
# <a name="getfederationinformationrequest-soap"></a><span data-ttu-id="47bf8-103">GetFederationInformationRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="47bf8-103">GetFederationInformationRequest (SOAP)</span></span>

<span data-ttu-id="47bf8-104">**GetFederationInformationRequest**要素は、 [GETFEDERATIONINFORMATION 操作 (SOAP)](getfederationinformation-operation-soap.md)操作の呼び出しのパラメーターを表します。</span><span class="sxs-lookup"><span data-stu-id="47bf8-104">The **GetFederationInformationRequest** element represents the parameters of a call to the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md)operation.</span></span>
  
```XML
<GetFederationInformationRequest>
   <Domain/>
</GetFederationInformationRequest>
```

<span data-ttu-id="47bf8-105">**GetFederationInformationRequest**</span><span class="sxs-lookup"><span data-stu-id="47bf8-105">**GetFederationInformationRequest**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="47bf8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="47bf8-106">Attributes and elements</span></span>

<span data-ttu-id="47bf8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="47bf8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47bf8-108">属性</span><span class="sxs-lookup"><span data-stu-id="47bf8-108">Attributes</span></span>

<span data-ttu-id="47bf8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="47bf8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47bf8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="47bf8-110">Child elements</span></span>

|<span data-ttu-id="47bf8-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="47bf8-111">**Element**</span></span>|<span data-ttu-id="47bf8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="47bf8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47bf8-113">ドメイン (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="47bf8-113">Domain (GetFederationInformation) (SOAP)</span></span>](domain-getfederationinformationsoap.md) <br/> |<span data-ttu-id="47bf8-114">フェデレーション信頼があるドメインを識別します。</span><span class="sxs-lookup"><span data-stu-id="47bf8-114">Identifies the domain that has a federation trust.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="47bf8-115">親要素</span><span class="sxs-lookup"><span data-stu-id="47bf8-115">Parent elements</span></span>

<span data-ttu-id="47bf8-116">なし。</span><span class="sxs-lookup"><span data-stu-id="47bf8-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="47bf8-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="47bf8-117">Text value</span></span>

<span data-ttu-id="47bf8-118">なし。</span><span class="sxs-lookup"><span data-stu-id="47bf8-118">None.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="47bf8-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="47bf8-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47bf8-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="47bf8-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="47bf8-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="47bf8-121">Schema Name</span></span>  <br/> |<span data-ttu-id="47bf8-122">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="47bf8-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="47bf8-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="47bf8-123">Validation File</span></span>  <br/> |<span data-ttu-id="47bf8-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="47bf8-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="47bf8-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="47bf8-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="47bf8-126">正しい</span><span class="sxs-lookup"><span data-stu-id="47bf8-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47bf8-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="47bf8-127">See also</span></span>

- [<span data-ttu-id="47bf8-128">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="47bf8-128">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

