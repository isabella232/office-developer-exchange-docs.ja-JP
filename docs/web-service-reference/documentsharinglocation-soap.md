---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: DocumentSharingLocation 要素には、ドキュメント共有場所の場所とメタデータ情報が含まれています。
ms.openlocfilehash: 6fed933da979ab3e3fca51ba606127b7f0a4e3f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457061"
---
# <a name="documentsharinglocation-soap"></a><span data-ttu-id="9ef0e-103">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ef0e-103">DocumentSharingLocation (SOAP)</span></span>

<span data-ttu-id="9ef0e-104">**Documentsharinglocation**要素には、ドキュメント共有場所の場所とメタデータ情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-104">The **DocumentSharingLocation** element contains location and metadata information for a document sharing location.</span></span> 
  
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

 <span data-ttu-id="9ef0e-105">**DocumentSharingLocation**</span><span class="sxs-lookup"><span data-stu-id="9ef0e-105">**DocumentSharingLocation**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ef0e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9ef0e-106">Attributes and elements</span></span>

<span data-ttu-id="9ef0e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ef0e-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ef0e-108">Attributes</span></span>

<span data-ttu-id="9ef0e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ef0e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9ef0e-110">Child elements</span></span>

|<span data-ttu-id="9ef0e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9ef0e-111">**Element**</span></span>|<span data-ttu-id="9ef0e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ef0e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ef0e-113">ServiceUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ef0e-113">ServiceUrl (SOAP)</span></span>](serviceurl-soap.md) <br/> |<span data-ttu-id="9ef0e-114">ドキュメント共有 web サービスの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-114">Represents the URL of the document sharing web service.</span></span>  <br/> |
|[<span data-ttu-id="9ef0e-115">LocationUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ef0e-115">LocationUrl (SOAP)</span></span>](locationurl-soap.md) <br/> |<span data-ttu-id="9ef0e-116">ドキュメント共有の場所の URL を表します。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-116">Represents the URL of the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="9ef0e-117">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ef0e-117">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="9ef0e-118">UI で使用するドキュメントの共有場所の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-118">Represents the name of the document sharing location to use in the UI.</span></span>  <br/> |
|[<span data-ttu-id="9ef0e-119">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ef0e-119">SupportedFileExtensions (SOAP)</span></span>](supportedfileextensions-soap.md) <br/> |<span data-ttu-id="9ef0e-120">文書の共有の場所に保存できるファイル拡張子を表します。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-120">Represents the file extensions that can be stored in the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="9ef0e-121">ExternalAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ef0e-121">ExternalAccessAllowed (SOAP)</span></span>](externalaccessallowed-soap.md) <br/> |<span data-ttu-id="9ef0e-122">外部接続でドキュメントの共有場所を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-122">Indicates whether the document sharing location is available to outside connections.</span></span>  <br/> |
|[<span data-ttu-id="9ef0e-123">AnonymousAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ef0e-123">AnonymousAccessAllowed (SOAP)</span></span>](anonymousaccessallowed-soap.md) <br/> |<span data-ttu-id="9ef0e-124">共有場所へのアクセスが認証済みユーザーを必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-124">Indicates whether access to the sharing location requires an authenticated user.</span></span>  <br/> |
|[<span data-ttu-id="9ef0e-125">CanModifyPermissions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ef0e-125">CanModifyPermissions (SOAP)</span></span>](canmodifypermissions-soap.md) <br/> |<span data-ttu-id="9ef0e-126">ユーザーがドキュメント共有の場所に対するアクセス許可を変更できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-126">Indicates whether the user can modify access permissions to the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="9ef0e-127">IsDefault (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ef0e-127">IsDefault (SOAP)</span></span>](isdefault-soap.md) <br/> |<span data-ttu-id="9ef0e-128">ドキュメントの共有場所がユーザーの既定の共有場所であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-128">Indicates whether the document sharing location is the user's default sharing location.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ef0e-129">親要素</span><span class="sxs-lookup"><span data-stu-id="9ef0e-129">Parent elements</span></span>

|<span data-ttu-id="9ef0e-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ef0e-130">**Element**</span></span>|<span data-ttu-id="9ef0e-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ef0e-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ef0e-132">DocumentSharingLocations (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ef0e-132">DocumentSharingLocations (SOAP)</span></span>](documentsharinglocations-soap.md) <br/> |<span data-ttu-id="9ef0e-133">ドキュメント共有の場所とメタデータの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-133">Contains a list of document sharing locations and metadata.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9ef0e-134">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9ef0e-134">Text value</span></span>

<span data-ttu-id="9ef0e-135">なし。</span><span class="sxs-lookup"><span data-stu-id="9ef0e-135">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ef0e-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9ef0e-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ef0e-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="9ef0e-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="9ef0e-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9ef0e-138">Schema Name</span></span>  <br/> |<span data-ttu-id="9ef0e-139">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="9ef0e-139">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="9ef0e-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9ef0e-140">Validation File</span></span>  <br/> |<span data-ttu-id="9ef0e-141">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9ef0e-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9ef0e-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9ef0e-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ef0e-143">正しい</span><span class="sxs-lookup"><span data-stu-id="9ef0e-143">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ef0e-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ef0e-144">See also</span></span>

- [<span data-ttu-id="9ef0e-145">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ef0e-145">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="9ef0e-146">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="9ef0e-146">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="9ef0e-147">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="9ef0e-147">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

