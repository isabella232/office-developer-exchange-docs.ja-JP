---
title: DocumentSharingLocationCollectionSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0e3346f9-7a55-4e87-b121-9b1ee7f227f4
description: DocumentSharingLocationCollectionSetting 要素は、ドキュメント共有の場所とメタデータのコレクションであるユーザー設定を表します。
ms.openlocfilehash: 2a52f639a1f1bf638aacc78666c58aed1fae0fa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457054"
---
# <a name="documentsharinglocationcollectionsetting-soap"></a><span data-ttu-id="51091-103">DocumentSharingLocationCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51091-103">DocumentSharingLocationCollectionSetting (SOAP)</span></span>

<span data-ttu-id="51091-104">**Documentsharinglocationcollectionsetting**要素は、ドキュメント共有の場所とメタデータのコレクションであるユーザー設定を表します。</span><span class="sxs-lookup"><span data-stu-id="51091-104">The **DocumentSharingLocationCollectionSetting** element represents a user setting that is a collection of documentation sharing locations and metadata.</span></span> 
  
[<span data-ttu-id="51091-105">DocumentSharingLocationCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51091-105">DocumentSharingLocationCollectionSetting (SOAP)</span></span>](documentsharinglocationcollectionsetting-soap.md)
  
```XML
<DocumentSharingLocationCollectionSetting>
    <DocumentSharingLocations />
</DocumentSharingLocationCollectionSetting>
```

 <span data-ttu-id="51091-106">**DocumentSharingLocationCollectionSetting**</span><span class="sxs-lookup"><span data-stu-id="51091-106">**DocumentSharingLocationCollectionSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51091-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="51091-107">Attributes and elements</span></span>

<span data-ttu-id="51091-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="51091-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51091-109">属性</span><span class="sxs-lookup"><span data-stu-id="51091-109">Attributes</span></span>

<span data-ttu-id="51091-110">なし。</span><span class="sxs-lookup"><span data-stu-id="51091-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51091-111">子要素</span><span class="sxs-lookup"><span data-stu-id="51091-111">Child elements</span></span>

|<span data-ttu-id="51091-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="51091-112">**Element**</span></span>|<span data-ttu-id="51091-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="51091-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51091-114">DocumentSharingLocations (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51091-114">DocumentSharingLocations (SOAP)</span></span>](documentsharinglocations-soap.md) <br/> |<span data-ttu-id="51091-115">ドキュメント共有の場所のリストの場所とメタデータを表します。</span><span class="sxs-lookup"><span data-stu-id="51091-115">Represents the location and metadata for a list of document sharing locations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="51091-116">親要素</span><span class="sxs-lookup"><span data-stu-id="51091-116">Parent elements</span></span>

|<span data-ttu-id="51091-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="51091-117">**Element**</span></span>|<span data-ttu-id="51091-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="51091-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51091-119">UserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51091-119">UserSettings (SOAP)</span></span>](usersettings-soap.md) <br/> |<span data-ttu-id="51091-120">ユーザー設定のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="51091-120">Represents a collection of user settings.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="51091-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="51091-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51091-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="51091-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="51091-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="51091-123">Schema Name</span></span>  <br/> |<span data-ttu-id="51091-124">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="51091-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="51091-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="51091-125">Validation File</span></span>  <br/> |<span data-ttu-id="51091-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="51091-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="51091-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="51091-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="51091-128">正しい</span><span class="sxs-lookup"><span data-stu-id="51091-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51091-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="51091-129">See also</span></span>

- [<span data-ttu-id="51091-130">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51091-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="51091-131">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="51091-131">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="51091-132">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="51091-132">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

