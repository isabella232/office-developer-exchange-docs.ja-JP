---
title: AnonymousAccessAllowed (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: bf819a65-30f2-4881-a34f-cb30a9c2b6a7
description: AnonymousAccessAllowed 要素は、ドキュメント共有の場所に認証済みユーザーが必要かどうかを示します。
ms.openlocfilehash: b3ff22fbba603bbd74dc08a0dbb1d8687714fe7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466081"
---
# <a name="anonymousaccessallowed-soap"></a><span data-ttu-id="3a916-103">AnonymousAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3a916-103">AnonymousAccessAllowed (SOAP)</span></span>

<span data-ttu-id="3a916-104">**AnonymousAccessAllowed**要素は、ドキュメント共有の場所に認証済みユーザーが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3a916-104">The **AnonymousAccessAllowed** element indicates whether a document sharing location requires an authenticated user.</span></span> 
  
```XML
<AnonymousAccessAllowed /> 
```

 <span data-ttu-id="3a916-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3a916-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a916-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3a916-106">Attributes and elements</span></span>

<span data-ttu-id="3a916-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3a916-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a916-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a916-108">Attributes</span></span>

<span data-ttu-id="3a916-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3a916-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a916-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3a916-110">Child elements</span></span>

<span data-ttu-id="3a916-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3a916-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3a916-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3a916-112">Parent elements</span></span>

|<span data-ttu-id="3a916-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3a916-113">**Element**</span></span>|<span data-ttu-id="3a916-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3a916-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a916-115">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3a916-115">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="3a916-116">ドキュメント共有場所の場所とメタデータ情報を表します。</span><span class="sxs-lookup"><span data-stu-id="3a916-116">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3a916-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3a916-117">Text value</span></span>

<span data-ttu-id="3a916-118">**AnonymousAccessAllowed**要素の Boolean 値は、共有場所が認証済みユーザーを必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3a916-118">The Boolean value of the **AnonymousAccessAllowed** element indicates whether the sharing location requires an authenticated user.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="3a916-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3a916-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a916-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="3a916-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3a916-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3a916-121">Schema Name</span></span>  <br/> |<span data-ttu-id="3a916-122">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="3a916-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3a916-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3a916-123">Validation File</span></span>  <br/> |<span data-ttu-id="3a916-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3a916-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a916-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3a916-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a916-126">正しい</span><span class="sxs-lookup"><span data-stu-id="3a916-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a916-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="3a916-127">See also</span></span>

- [<span data-ttu-id="3a916-128">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3a916-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="3a916-129">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="3a916-129">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="3a916-130">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="3a916-130">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

