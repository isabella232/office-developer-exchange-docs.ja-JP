---
title: DocumentSharingLocations (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 394f6015-721b-4800-9286-039d430f09b3
description: DocumentSharingLocations 要素には、ドキュメント共有場所の場所とメタデータ情報の一覧が含まれています。
ms.openlocfilehash: af8b076c7a3bd26355a53457a43f4a5f86bf517e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457040"
---
# <a name="documentsharinglocations-soap"></a><span data-ttu-id="7c2ae-103">DocumentSharingLocations (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7c2ae-103">DocumentSharingLocations (SOAP)</span></span>

<span data-ttu-id="7c2ae-104">**Documentsharinglocations**要素には、ドキュメント共有場所の場所とメタデータ情報の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7c2ae-104">The **DocumentSharingLocations** element contains a list of location and metadata information for a document sharing location.</span></span> 
  
```XML
<DocumentSharingLocations>
   <DocumentSharingLocation />
</DocumentSharingLocations>
```

 <span data-ttu-id="7c2ae-105">**DocumentSharingLocations**</span><span class="sxs-lookup"><span data-stu-id="7c2ae-105">**DocumentSharingLocations**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c2ae-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7c2ae-106">Attributes and elements</span></span>

<span data-ttu-id="7c2ae-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c2ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c2ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c2ae-108">Attributes</span></span>

<span data-ttu-id="7c2ae-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7c2ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c2ae-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7c2ae-110">Child elements</span></span>

|<span data-ttu-id="7c2ae-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7c2ae-111">**Element**</span></span>|<span data-ttu-id="7c2ae-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c2ae-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c2ae-113">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7c2ae-113">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="7c2ae-114">ドキュメント共有の場所の場所とメタデータが保存されています。</span><span class="sxs-lookup"><span data-stu-id="7c2ae-114">Contains the location and metadata for a document sharing location.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c2ae-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7c2ae-115">Parent elements</span></span>

|<span data-ttu-id="7c2ae-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7c2ae-116">**Element**</span></span>|<span data-ttu-id="7c2ae-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c2ae-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c2ae-118">DocumentSharingLocationCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7c2ae-118">DocumentSharingLocationCollectionSetting (SOAP)</span></span>](documentsharinglocationcollectionsetting-soap.md) <br/> |<span data-ttu-id="7c2ae-119">ドキュメント共有の場所とメタデータのコレクションであるユーザー設定を表します。</span><span class="sxs-lookup"><span data-stu-id="7c2ae-119">Represents a user setting that is a collection of documentation sharing locations and metadata.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="7c2ae-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7c2ae-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c2ae-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="7c2ae-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="7c2ae-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7c2ae-122">Schema Name</span></span>  <br/> |<span data-ttu-id="7c2ae-123">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="7c2ae-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="7c2ae-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7c2ae-124">Validation File</span></span>  <br/> |<span data-ttu-id="7c2ae-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7c2ae-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7c2ae-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7c2ae-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c2ae-127">正しい</span><span class="sxs-lookup"><span data-stu-id="7c2ae-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c2ae-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="7c2ae-128">See also</span></span>

- [<span data-ttu-id="7c2ae-129">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7c2ae-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="7c2ae-130">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="7c2ae-130">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="7c2ae-131">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="7c2ae-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

