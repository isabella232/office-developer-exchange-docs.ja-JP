---
title: SupportedFileExtensions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 6f73d18c-7bb1-4ab6-a23b-6d948e590b53
description: SupportedFileExtensions 要素には、ドキュメントの共有の場所に保存できるファイル拡張子が表示されます。
ms.openlocfilehash: d783b147a25ebbe3bff59c2142012b50bd80004e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44433988"
---
# <a name="supportedfileextensions-soap"></a><span data-ttu-id="dc0e4-103">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dc0e4-103">SupportedFileExtensions (SOAP)</span></span>

<span data-ttu-id="dc0e4-104">**SupportedFileExtensions**要素には、ドキュメントの共有の場所に保存できるファイル拡張子が表示されます。</span><span class="sxs-lookup"><span data-stu-id="dc0e4-104">The **SupportedFileExtensions** element lists the file extensions that can be stored in a document sharing location.</span></span> 
  
```XML
<SupportedFileExtensions /> 
```

 <span data-ttu-id="dc0e4-105">**ArrayOfFileExtension**</span><span class="sxs-lookup"><span data-stu-id="dc0e4-105">**ArrayOfFileExtension**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc0e4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dc0e4-106">Attributes and elements</span></span>

<span data-ttu-id="dc0e4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dc0e4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc0e4-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc0e4-108">Attributes</span></span>

<span data-ttu-id="dc0e4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dc0e4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc0e4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dc0e4-110">Child elements</span></span>

|<span data-ttu-id="dc0e4-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="dc0e4-111">**Element**</span></span>|<span data-ttu-id="dc0e4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dc0e4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc0e4-113">FileExtension (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dc0e4-113">FileExtension (SOAP)</span></span>](fileextension-soap.md) <br/> |<span data-ttu-id="dc0e4-114">ファイル拡張子を表します。</span><span class="sxs-lookup"><span data-stu-id="dc0e4-114">Represents a file extension.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dc0e4-115">親要素</span><span class="sxs-lookup"><span data-stu-id="dc0e4-115">Parent elements</span></span>

|<span data-ttu-id="dc0e4-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="dc0e4-116">**Element**</span></span>|<span data-ttu-id="dc0e4-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="dc0e4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc0e4-118">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dc0e4-118">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="dc0e4-119">ドキュメント共有場所の場所とメタデータ情報を表します。</span><span class="sxs-lookup"><span data-stu-id="dc0e4-119">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="dc0e4-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dc0e4-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc0e4-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="dc0e4-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="dc0e4-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dc0e4-122">Schema Name</span></span>  <br/> |<span data-ttu-id="dc0e4-123">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="dc0e4-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="dc0e4-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dc0e4-124">Validation File</span></span>  <br/> |<span data-ttu-id="dc0e4-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="dc0e4-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dc0e4-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dc0e4-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc0e4-127">正しい</span><span class="sxs-lookup"><span data-stu-id="dc0e4-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc0e4-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="dc0e4-128">See also</span></span>



[<span data-ttu-id="dc0e4-129">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dc0e4-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="dc0e4-130">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="dc0e4-130">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="dc0e4-131">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="dc0e4-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

