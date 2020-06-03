---
title: ServerVersionInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerVersionInfo
api_type:
- schema
ms.assetid: c04a6872-ca27-432b-aac2-36b023d0afc6
description: ServerVersionInfo 要素は、Microsoft Exchange Server のバージョン番号を表します。
ms.openlocfilehash: 5bd1fbd8fdee584a9d272fa8ab82f2a31c1357fe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466830"
---
# <a name="serverversioninfo"></a><span data-ttu-id="b509a-103">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b509a-103">ServerVersionInfo</span></span>

<span data-ttu-id="b509a-104">**ServerVersionInfo**要素は、Microsoft Exchange Server のバージョン番号を表します。</span><span class="sxs-lookup"><span data-stu-id="b509a-104">The **ServerVersionInfo** element represents the Microsoft Exchange Server version number.</span></span> 
  
```xml
<ServerVersionInfo MajorVersion="" MinorVersion="" MajorBuildNumber="" MinorBuildNumber="" Version="" />
```

## <a name="attributes-and-elements"></a><span data-ttu-id="b509a-105">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b509a-105">Attributes and elements</span></span>

<span data-ttu-id="b509a-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b509a-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b509a-107">属性</span><span class="sxs-lookup"><span data-stu-id="b509a-107">Attributes</span></span>

|<span data-ttu-id="b509a-108">**属性**</span><span class="sxs-lookup"><span data-stu-id="b509a-108">**Attribute**</span></span>|<span data-ttu-id="b509a-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="b509a-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b509a-110">MajorVersion</span><span class="sxs-lookup"><span data-stu-id="b509a-110">MajorVersion</span></span>  <br/> |<span data-ttu-id="b509a-111">メジャーバージョン番号について説明します。</span><span class="sxs-lookup"><span data-stu-id="b509a-111">Describes the major version number.</span></span>  <br/> |
|<span data-ttu-id="b509a-112">MinorVersion</span><span class="sxs-lookup"><span data-stu-id="b509a-112">MinorVersion</span></span>  <br/> |<span data-ttu-id="b509a-113">マイナーバージョン番号を記述します。</span><span class="sxs-lookup"><span data-stu-id="b509a-113">Describes the minor version number.</span></span>  <br/> |
|<span data-ttu-id="b509a-114">MajorBuildNumber</span><span class="sxs-lookup"><span data-stu-id="b509a-114">MajorBuildNumber</span></span>  <br/> |<span data-ttu-id="b509a-115">主要なビルド番号を記述します。</span><span class="sxs-lookup"><span data-stu-id="b509a-115">Describes the major build number.</span></span>  <br/> |
|<span data-ttu-id="b509a-116">MinorBuildNumber または</span><span class="sxs-lookup"><span data-stu-id="b509a-116">MinorBuildNumber</span></span>  <br/> |<span data-ttu-id="b509a-117">マイナービルド番号を記述します。</span><span class="sxs-lookup"><span data-stu-id="b509a-117">Describes the minor build number.</span></span>  <br/> |
|<span data-ttu-id="b509a-118">バージョン</span><span class="sxs-lookup"><span data-stu-id="b509a-118">Version</span></span>  <br/> |<span data-ttu-id="b509a-119">Exchange Web サービス (EWS) スキーマのバージョンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b509a-119">Describes the Exchange Web Services (EWS) schema version.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b509a-120">子要素</span><span class="sxs-lookup"><span data-stu-id="b509a-120">Child elements</span></span>

<span data-ttu-id="b509a-121">なし。</span><span class="sxs-lookup"><span data-stu-id="b509a-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b509a-122">親要素</span><span class="sxs-lookup"><span data-stu-id="b509a-122">Parent elements</span></span>

<span data-ttu-id="b509a-123">なし。</span><span class="sxs-lookup"><span data-stu-id="b509a-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b509a-124">注釈</span><span class="sxs-lookup"><span data-stu-id="b509a-124">Remarks</span></span>

<span data-ttu-id="b509a-125">この要素は、Exchange Web サービス応答メッセージの SOAP ヘッダーで返されます。</span><span class="sxs-lookup"><span data-stu-id="b509a-125">This element is returned in the SOAP header of an Exchange Web Services response message.</span></span>
  
<span data-ttu-id="b509a-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b509a-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b509a-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b509a-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b509a-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="b509a-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b509a-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b509a-129">Schema Name</span></span>  <br/> |<span data-ttu-id="b509a-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b509a-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="b509a-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b509a-131">Validation File</span></span>  <br/> |<span data-ttu-id="b509a-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b509a-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b509a-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b509a-133">Can Be Empty</span></span>  <br/> |<span data-ttu-id="b509a-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="b509a-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b509a-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="b509a-135">See also</span></span>



- [<span data-ttu-id="b509a-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b509a-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

