---
title: DocumentSharingLocationCollectionSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0e3346f9-7a55-4e87-b121-9b1ee7f227f4
description: DocumentSharingLocationCollectionSetting 要素は、ドキュメントの共有の場所およびメタデータのコレクションに設定されているユーザーを表します。
ms.openlocfilehash: 9871e3fccdcce95fc275768d99159c70f57a07af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760139"
---
# <a name="documentsharinglocationcollectionsetting-soap"></a><span data-ttu-id="e9433-103">DocumentSharingLocationCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e9433-103">DocumentSharingLocationCollectionSetting (SOAP)</span></span>

<span data-ttu-id="e9433-104">**DocumentSharingLocationCollectionSetting**要素は、ドキュメントの共有の場所およびメタデータのコレクションに設定されているユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="e9433-104">The **DocumentSharingLocationCollectionSetting** element represents a user setting that is a collection of documentation sharing locations and metadata.</span></span> 
  
[<span data-ttu-id="e9433-105">DocumentSharingLocationCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e9433-105">DocumentSharingLocationCollectionSetting (SOAP)</span></span>](documentsharinglocationcollectionsetting-soap.md)
  
```XML
<DocumentSharingLocationCollectionSetting>
    <DocumentSharingLocations />
</DocumentSharingLocationCollectionSetting>
```

 <span data-ttu-id="e9433-106">**DocumentSharingLocationCollectionSetting**</span><span class="sxs-lookup"><span data-stu-id="e9433-106">**DocumentSharingLocationCollectionSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9433-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e9433-107">Attributes and elements</span></span>

<span data-ttu-id="e9433-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9433-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9433-109">属性</span><span class="sxs-lookup"><span data-stu-id="e9433-109">Attributes</span></span>

<span data-ttu-id="e9433-110">なし。</span><span class="sxs-lookup"><span data-stu-id="e9433-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9433-111">子要素</span><span class="sxs-lookup"><span data-stu-id="e9433-111">Child elements</span></span>

|<span data-ttu-id="e9433-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="e9433-112">**Element**</span></span>|<span data-ttu-id="e9433-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9433-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9433-114">DocumentSharingLocations (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e9433-114">DocumentSharingLocations (SOAP)</span></span>](documentsharinglocations-soap.md) <br/> |<span data-ttu-id="e9433-115">位置とドキュメントの共有の場所のリストのメタデータを表します。</span><span class="sxs-lookup"><span data-stu-id="e9433-115">Represents the location and metadata for a list of document sharing locations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9433-116">親要素</span><span class="sxs-lookup"><span data-stu-id="e9433-116">Parent elements</span></span>

|<span data-ttu-id="e9433-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="e9433-117">**Element**</span></span>|<span data-ttu-id="e9433-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9433-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9433-119">ユーザー (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e9433-119">UserSettings (SOAP)</span></span>](usersettings-soap.md) <br/> |<span data-ttu-id="e9433-120">ユーザー設定のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e9433-120">Represents a collection of user settings.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="e9433-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="e9433-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9433-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="e9433-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e9433-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9433-123">Schema Name</span></span>  <br/> |<span data-ttu-id="e9433-124">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="e9433-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e9433-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9433-125">Validation File</span></span>  <br/> |<span data-ttu-id="e9433-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e9433-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e9433-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e9433-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9433-128">True</span><span class="sxs-lookup"><span data-stu-id="e9433-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9433-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9433-129">See also</span></span>

- [<span data-ttu-id="e9433-130">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e9433-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="e9433-131">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="e9433-131">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="e9433-132">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="e9433-132">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

