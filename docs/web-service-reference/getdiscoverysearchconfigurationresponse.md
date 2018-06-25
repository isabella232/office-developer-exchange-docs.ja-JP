---
title: GetDiscoverySearchConfigurationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d963e6c-e94d-462b-8c44-95d55c848fb2
description: GetDiscoverySearchConfigurationResponse 要素は、GetDiscoverySearchConfiguration 要求への応答を指定します。
ms.openlocfilehash: 6f4bbc05da0c2883f78b31cb46108e993b8b8fdd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760694"
---
# <a name="getdiscoverysearchconfigurationresponse"></a><span data-ttu-id="9b50e-103">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="9b50e-103">GetDiscoverySearchConfigurationResponse</span></span>

<span data-ttu-id="9b50e-104">**GetDiscoverySearchConfigurationResponse**要素は、 **GetDiscoverySearchConfiguration**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b50e-104">The **GetDiscoverySearchConfigurationResponse** element specifies the response to a **GetDiscoverySearchConfiguration** request.</span></span> 
  
```XML
<GetDiscoverySearchConfigurationResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DiscoverySearchConfigurations/>
</GetDiscoverySearchConfigurationResponse>
```

 <span data-ttu-id="9b50e-105">**GetDiscoverySearchConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9b50e-105">**GetDiscoverySearchConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b50e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9b50e-106">Attributes and elements</span></span>

<span data-ttu-id="9b50e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9b50e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b50e-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b50e-108">Attributes</span></span>

<span data-ttu-id="9b50e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9b50e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b50e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9b50e-110">Child elements</span></span>

<span data-ttu-id="9b50e-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [DiscoverySearchConfigurations](discoverysearchconfigurations.md)</span><span class="sxs-lookup"><span data-stu-id="9b50e-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [DiscoverySearchConfigurations](discoverysearchconfigurations.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9b50e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9b50e-112">Parent elements</span></span>

[<span data-ttu-id="9b50e-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9b50e-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="9b50e-114">備考</span><span class="sxs-lookup"><span data-stu-id="9b50e-114">Remarks</span></span>

<span data-ttu-id="9b50e-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9b50e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9b50e-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9b50e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b50e-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="9b50e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b50e-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="9b50e-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9b50e-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9b50e-119">Schema name</span></span>  <br/> |<span data-ttu-id="9b50e-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9b50e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9b50e-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9b50e-121">Validation file</span></span>  <br/> |<span data-ttu-id="9b50e-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9b50e-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9b50e-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9b50e-123">Can be empty</span></span>  <br/> |<span data-ttu-id="9b50e-124">false</span><span class="sxs-lookup"><span data-stu-id="9b50e-124">false</span></span>  <br/> |
   

