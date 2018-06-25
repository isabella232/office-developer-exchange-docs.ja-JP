---
title: CanModifyPermissions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9693de1a-0c76-4898-8f4d-a8693fb005b3
description: CanModifyPermissions 要素は、ユーザーが共有ドキュメントへのアクセス許可を変更できるかどうかを示します。
ms.openlocfilehash: 16526cb79eeca591af6e009e67959a1c3b58a5d7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759608"
---
# <a name="canmodifypermissions-soap"></a><span data-ttu-id="ba844-103">CanModifyPermissions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ba844-103">CanModifyPermissions (SOAP)</span></span>

<span data-ttu-id="ba844-104">**CanModifyPermissions**要素は、ユーザーが共有ドキュメントへのアクセス許可を変更できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ba844-104">The **CanModifyPermissions** element indicates whether a user can modify access permissions to a document sharing location.</span></span> 
  
```XML
<CanModifyPermissions /> 
```

 <span data-ttu-id="ba844-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="ba844-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba844-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ba844-106">Attributes and elements</span></span>

<span data-ttu-id="ba844-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ba844-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba844-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba844-108">Attributes</span></span>

<span data-ttu-id="ba844-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ba844-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba844-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ba844-110">Child elements</span></span>

<span data-ttu-id="ba844-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ba844-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba844-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ba844-112">Parent elements</span></span>

|<span data-ttu-id="ba844-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ba844-113">**Element**</span></span>|<span data-ttu-id="ba844-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ba844-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba844-115">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ba844-115">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="ba844-116">場所を共有するドキュメントの場所およびメタデータの情報を表します。</span><span class="sxs-lookup"><span data-stu-id="ba844-116">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ba844-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ba844-117">Text value</span></span>

<span data-ttu-id="ba844-118">**CanModifyPermissions**要素のブール値は、ユーザーが共有の場所へのアクセス許可を変更できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ba844-118">The Boolean value of the **CanModifyPermissions** element indicates whether users can modify access permissions to the sharing location.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ba844-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="ba844-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba844-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="ba844-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ba844-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ba844-121">Schema Name</span></span>  <br/> |<span data-ttu-id="ba844-122">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="ba844-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ba844-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ba844-123">Validation File</span></span>  <br/> |<span data-ttu-id="ba844-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ba844-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ba844-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ba844-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba844-126">True</span><span class="sxs-lookup"><span data-stu-id="ba844-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba844-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="ba844-127">See also</span></span>



[<span data-ttu-id="ba844-128">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ba844-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="ba844-129">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="ba844-129">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="ba844-130">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="ba844-130">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

