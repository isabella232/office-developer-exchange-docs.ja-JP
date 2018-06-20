---
title: SupportedFileExtensions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 6f73d18c-7bb1-4ab6-a23b-6d948e590b53
description: SupportedFileExtensions 要素には、場所を共有するドキュメントに格納できるファイルの拡張子が一覧表示されます。
ms.openlocfilehash: 0f1dbbce2b836fe05e4bc612c607302783d5e05d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839629"
---
# <a name="supportedfileextensions-soap"></a><span data-ttu-id="2d866-103">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2d866-103">SupportedFileExtensions (SOAP)</span></span>

<span data-ttu-id="2d866-104">**SupportedFileExtensions**要素には、場所を共有するドキュメントに格納できるファイルの拡張子が一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="2d866-104">The **SupportedFileExtensions** element lists the file extensions that can be stored in a document sharing location.</span></span> 
  
```XML
<SupportedFileExtensions /> 
```

 <span data-ttu-id="2d866-105">**ArrayOfFileExtension**</span><span class="sxs-lookup"><span data-stu-id="2d866-105">**ArrayOfFileExtension**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d866-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2d866-106">Attributes and elements</span></span>

<span data-ttu-id="2d866-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2d866-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d866-108">属性</span><span class="sxs-lookup"><span data-stu-id="2d866-108">Attributes</span></span>

<span data-ttu-id="2d866-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2d866-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d866-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2d866-110">Child elements</span></span>

|<span data-ttu-id="2d866-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2d866-111">**Element**</span></span>|<span data-ttu-id="2d866-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2d866-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d866-113">FileExtension (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2d866-113">FileExtension (SOAP)</span></span>](fileextension-soap.md) <br/> |<span data-ttu-id="2d866-114">ファイルの拡張子を表します。</span><span class="sxs-lookup"><span data-stu-id="2d866-114">Represents a file extension.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d866-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2d866-115">Parent elements</span></span>

|<span data-ttu-id="2d866-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="2d866-116">**Element**</span></span>|<span data-ttu-id="2d866-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="2d866-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d866-118">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2d866-118">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="2d866-119">場所を共有するドキュメントの場所およびメタデータの情報を表します。</span><span class="sxs-lookup"><span data-stu-id="2d866-119">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="2d866-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="2d866-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d866-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="2d866-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="2d866-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2d866-122">Schema Name</span></span>  <br/> |<span data-ttu-id="2d866-123">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="2d866-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="2d866-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2d866-124">Validation File</span></span>  <br/> |<span data-ttu-id="2d866-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2d866-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2d866-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2d866-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="2d866-127">True</span><span class="sxs-lookup"><span data-stu-id="2d866-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d866-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="2d866-128">See also</span></span>



[<span data-ttu-id="2d866-129">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2d866-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="2d866-130">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="2d866-130">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="2d866-131">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="2d866-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

