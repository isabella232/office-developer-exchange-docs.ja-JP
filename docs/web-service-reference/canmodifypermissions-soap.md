---
title: CanModifyPermissions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9693de1a-0c76-4898-8f4d-a8693fb005b3
description: CanModifyPermissions 要素は、ユーザーがドキュメント共有の場所に対するアクセス許可を変更できるかどうかを示します。
ms.openlocfilehash: bf21b80a738498176bac41feea001ff859a54c2b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461584"
---
# <a name="canmodifypermissions-soap"></a><span data-ttu-id="12a1f-103">CanModifyPermissions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="12a1f-103">CanModifyPermissions (SOAP)</span></span>

<span data-ttu-id="12a1f-104">**Canmodifypermissions**要素は、ユーザーがドキュメント共有の場所に対するアクセス許可を変更できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="12a1f-104">The **CanModifyPermissions** element indicates whether a user can modify access permissions to a document sharing location.</span></span> 
  
```XML
<CanModifyPermissions /> 
```

 <span data-ttu-id="12a1f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="12a1f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12a1f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="12a1f-106">Attributes and elements</span></span>

<span data-ttu-id="12a1f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="12a1f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12a1f-108">属性</span><span class="sxs-lookup"><span data-stu-id="12a1f-108">Attributes</span></span>

<span data-ttu-id="12a1f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="12a1f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12a1f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="12a1f-110">Child elements</span></span>

<span data-ttu-id="12a1f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="12a1f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="12a1f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="12a1f-112">Parent elements</span></span>

|<span data-ttu-id="12a1f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="12a1f-113">**Element**</span></span>|<span data-ttu-id="12a1f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="12a1f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12a1f-115">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="12a1f-115">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="12a1f-116">ドキュメント共有場所の場所とメタデータ情報を表します。</span><span class="sxs-lookup"><span data-stu-id="12a1f-116">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12a1f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="12a1f-117">Text value</span></span>

<span data-ttu-id="12a1f-118">**Canmodifypermissions**要素のブール値は、ユーザーが共有の場所に対するアクセス許可を変更できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="12a1f-118">The Boolean value of the **CanModifyPermissions** element indicates whether users can modify access permissions to the sharing location.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="12a1f-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="12a1f-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12a1f-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="12a1f-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="12a1f-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="12a1f-121">Schema Name</span></span>  <br/> |<span data-ttu-id="12a1f-122">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="12a1f-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="12a1f-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="12a1f-123">Validation File</span></span>  <br/> |<span data-ttu-id="12a1f-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="12a1f-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="12a1f-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="12a1f-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="12a1f-126">正しい</span><span class="sxs-lookup"><span data-stu-id="12a1f-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12a1f-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="12a1f-127">See also</span></span>



[<span data-ttu-id="12a1f-128">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="12a1f-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="12a1f-129">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="12a1f-129">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="12a1f-130">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="12a1f-130">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

