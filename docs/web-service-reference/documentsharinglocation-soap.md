---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: DocumentSharingLocation 要素には、場所と場所を共有するドキュメントのメタデータ情報が含まれています。
ms.openlocfilehash: d258efecb46d570138c7c2c78ed9d2fa9a275103
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760140"
---
# <a name="documentsharinglocation-soap"></a><span data-ttu-id="44023-103">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44023-103">DocumentSharingLocation (SOAP)</span></span>

<span data-ttu-id="44023-104">**DocumentSharingLocation**要素には、場所と場所を共有するドキュメントのメタデータ情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="44023-104">The **DocumentSharingLocation** element contains location and metadata information for a document sharing location.</span></span> 
  
```XML
<DocumentSharingLocation>
   <ServiceUrl />
   <LocationUrl />
   <DisplayName />
   <SupportedFileExtensions />
   <ExternalAccessAllowed />
   <AnonymousAccessAllowed />
   <CanModifyPermissions />
   <IsDefault />
</DocumentSharingLocation>
```

 <span data-ttu-id="44023-105">**DocumentSharingLocation**</span><span class="sxs-lookup"><span data-stu-id="44023-105">**DocumentSharingLocation**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="44023-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="44023-106">Attributes and elements</span></span>

<span data-ttu-id="44023-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="44023-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44023-108">属性</span><span class="sxs-lookup"><span data-stu-id="44023-108">Attributes</span></span>

<span data-ttu-id="44023-109">なし。</span><span class="sxs-lookup"><span data-stu-id="44023-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44023-110">子要素</span><span class="sxs-lookup"><span data-stu-id="44023-110">Child elements</span></span>

|<span data-ttu-id="44023-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="44023-111">**Element**</span></span>|<span data-ttu-id="44023-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="44023-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44023-113">ServiceUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44023-113">ServiceUrl (SOAP)</span></span>](serviceurl-soap.md) <br/> |<span data-ttu-id="44023-114">Web サービスを共有するドキュメントの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="44023-114">Represents the URL of the document sharing web service.</span></span>  <br/> |
|[<span data-ttu-id="44023-115">LocationUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44023-115">LocationUrl (SOAP)</span></span>](locationurl-soap.md) <br/> |<span data-ttu-id="44023-116">ドキュメント共有の場所の URL を表します。</span><span class="sxs-lookup"><span data-stu-id="44023-116">Represents the URL of the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="44023-117">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44023-117">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="44023-118">UI で使用する場所を共有するドキュメントの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="44023-118">Represents the name of the document sharing location to use in the UI.</span></span>  <br/> |
|[<span data-ttu-id="44023-119">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44023-119">SupportedFileExtensions (SOAP)</span></span>](supportedfileextensions-soap.md) <br/> |<span data-ttu-id="44023-120">ドキュメント共有の場所に格納できるファイルの拡張子を表します。</span><span class="sxs-lookup"><span data-stu-id="44023-120">Represents the file extensions that can be stored in the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="44023-121">ExternalAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44023-121">ExternalAccessAllowed (SOAP)</span></span>](externalaccessallowed-soap.md) <br/> |<span data-ttu-id="44023-122">ドキュメント共有の場所は外部の接続からに使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="44023-122">Indicates whether the document sharing location is available to outside connections.</span></span>  <br/> |
|[<span data-ttu-id="44023-123">AnonymousAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44023-123">AnonymousAccessAllowed (SOAP)</span></span>](anonymousaccessallowed-soap.md) <br/> |<span data-ttu-id="44023-124">共有場所へのアクセスに認証されたユーザーが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="44023-124">Indicates whether access to the sharing location requires an authenticated user.</span></span>  <br/> |
|[<span data-ttu-id="44023-125">CanModifyPermissions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44023-125">CanModifyPermissions (SOAP)</span></span>](canmodifypermissions-soap.md) <br/> |<span data-ttu-id="44023-126">ユーザーがドキュメントの場所を共有するアクセス許可を変更できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="44023-126">Indicates whether the user can modify access permissions to the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="44023-127">IsDefault (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44023-127">IsDefault (SOAP)</span></span>](isdefault-soap.md) <br/> |<span data-ttu-id="44023-128">ドキュメントの場所を共有は、ユーザーの既定の場所を共有するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="44023-128">Indicates whether the document sharing location is the user's default sharing location.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="44023-129">親要素</span><span class="sxs-lookup"><span data-stu-id="44023-129">Parent elements</span></span>

|<span data-ttu-id="44023-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="44023-130">**Element**</span></span>|<span data-ttu-id="44023-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="44023-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44023-132">DocumentSharingLocations (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44023-132">DocumentSharingLocations (SOAP)</span></span>](documentsharinglocations-soap.md) <br/> |<span data-ttu-id="44023-133">ドキュメントの場所およびメタデータの共有の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="44023-133">Contains a list of document sharing locations and metadata.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="44023-134">テキスト値</span><span class="sxs-lookup"><span data-stu-id="44023-134">Text value</span></span>

<span data-ttu-id="44023-135">なし。</span><span class="sxs-lookup"><span data-stu-id="44023-135">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44023-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="44023-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44023-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="44023-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="44023-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="44023-138">Schema Name</span></span>  <br/> |<span data-ttu-id="44023-139">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="44023-139">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="44023-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="44023-140">Validation File</span></span>  <br/> |<span data-ttu-id="44023-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="44023-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="44023-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="44023-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="44023-143">True</span><span class="sxs-lookup"><span data-stu-id="44023-143">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44023-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="44023-144">See also</span></span>

- [<span data-ttu-id="44023-145">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="44023-145">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="44023-146">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="44023-146">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="44023-147">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="44023-147">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

