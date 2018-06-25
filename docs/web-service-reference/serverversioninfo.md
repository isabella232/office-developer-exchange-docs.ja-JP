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
ms.openlocfilehash: aff8a6542e2ae6fb1148dd29051b7b33ad90eeff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833389"
---
# <a name="serverversioninfo"></a><span data-ttu-id="ae8d6-103">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ae8d6-103">ServerVersionInfo</span></span>

<span data-ttu-id="ae8d6-104">**ServerVersionInfo**要素は、Microsoft Exchange Server のバージョン番号を表します。</span><span class="sxs-lookup"><span data-stu-id="ae8d6-104">The **ServerVersionInfo** element represents the Microsoft Exchange Server version number.</span></span> 
  
```xml
<ServerVersionInfo MajorVersion="" MinorVersion="" MajorBuildNumber="" MinorBuildNumber="" Version="" />
```

## <a name="attributes-and-elements"></a><span data-ttu-id="ae8d6-105">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ae8d6-105">Attributes and elements</span></span>

<span data-ttu-id="ae8d6-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ae8d6-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae8d6-107">属性</span><span class="sxs-lookup"><span data-stu-id="ae8d6-107">Attributes</span></span>

|<span data-ttu-id="ae8d6-108">**属性**</span><span class="sxs-lookup"><span data-stu-id="ae8d6-108">**Attribute**</span></span>|<span data-ttu-id="ae8d6-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae8d6-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ae8d6-110">MajorVersion</span><span class="sxs-lookup"><span data-stu-id="ae8d6-110">MajorVersion</span></span>  <br/> |<span data-ttu-id="ae8d6-111">メジャー バージョン番号をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ae8d6-111">Describes the major version number.</span></span>  <br/> |
|<span data-ttu-id="ae8d6-112">MinorVersion</span><span class="sxs-lookup"><span data-stu-id="ae8d6-112">MinorVersion</span></span>  <br/> |<span data-ttu-id="ae8d6-113">マイナー バージョン番号をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ae8d6-113">Describes the minor version number.</span></span>  <br/> |
|<span data-ttu-id="ae8d6-114">MajorBuildNumber</span><span class="sxs-lookup"><span data-stu-id="ae8d6-114">MajorBuildNumber</span></span>  <br/> |<span data-ttu-id="ae8d6-115">メジャー ビルド番号をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ae8d6-115">Describes the major build number.</span></span>  <br/> |
|<span data-ttu-id="ae8d6-116">MinorBuildNumber</span><span class="sxs-lookup"><span data-stu-id="ae8d6-116">MinorBuildNumber</span></span>  <br/> |<span data-ttu-id="ae8d6-117">マイナー ビルド番号をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ae8d6-117">Describes the minor build number.</span></span>  <br/> |
|<span data-ttu-id="ae8d6-118">バージョン</span><span class="sxs-lookup"><span data-stu-id="ae8d6-118">Version</span></span>  <br/> |<span data-ttu-id="ae8d6-119">Exchange Web サービス (EWS) スキーマのバージョンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ae8d6-119">Describes the Exchange Web Services (EWS) schema version.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ae8d6-120">子要素</span><span class="sxs-lookup"><span data-stu-id="ae8d6-120">Child elements</span></span>

<span data-ttu-id="ae8d6-121">なし。</span><span class="sxs-lookup"><span data-stu-id="ae8d6-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ae8d6-122">親要素</span><span class="sxs-lookup"><span data-stu-id="ae8d6-122">Parent elements</span></span>

<span data-ttu-id="ae8d6-123">なし。</span><span class="sxs-lookup"><span data-stu-id="ae8d6-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae8d6-124">備考</span><span class="sxs-lookup"><span data-stu-id="ae8d6-124">Remarks</span></span>

<span data-ttu-id="ae8d6-125">この要素は、Exchange Web サービスの応答メッセージの SOAP ヘッダーで返されます。</span><span class="sxs-lookup"><span data-stu-id="ae8d6-125">This element is returned in the SOAP header of an Exchange Web Services response message.</span></span>
  
<span data-ttu-id="ae8d6-126">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ae8d6-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ae8d6-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="ae8d6-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae8d6-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="ae8d6-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ae8d6-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ae8d6-129">Schema Name</span></span>  <br/> |<span data-ttu-id="ae8d6-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ae8d6-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="ae8d6-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ae8d6-131">Validation File</span></span>  <br/> |<span data-ttu-id="ae8d6-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ae8d6-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae8d6-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ae8d6-133">Can Be Empty</span></span>  <br/> |<span data-ttu-id="ae8d6-134">False</span><span class="sxs-lookup"><span data-stu-id="ae8d6-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae8d6-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="ae8d6-135">See also</span></span>



- [<span data-ttu-id="ae8d6-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ae8d6-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

