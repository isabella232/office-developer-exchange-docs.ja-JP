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
ms.openlocfilehash: 98393943434b5e3460485b7d75c2b5285983f597
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460982"
---
# <a name="getdiscoverysearchconfigurationresponse"></a><span data-ttu-id="70749-103">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="70749-103">GetDiscoverySearchConfigurationResponse</span></span>

<span data-ttu-id="70749-104">**GetDiscoverySearchConfigurationResponse**要素は、 **Getdiscoverysearchconfiguration**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="70749-104">The **GetDiscoverySearchConfigurationResponse** element specifies the response to a **GetDiscoverySearchConfiguration** request.</span></span> 
  
```XML
<GetDiscoverySearchConfigurationResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DiscoverySearchConfigurations/>
</GetDiscoverySearchConfigurationResponse>
```

 <span data-ttu-id="70749-105">**GetDiscoverySearchConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="70749-105">**GetDiscoverySearchConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70749-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="70749-106">Attributes and elements</span></span>

<span data-ttu-id="70749-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="70749-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70749-108">属性</span><span class="sxs-lookup"><span data-stu-id="70749-108">Attributes</span></span>

<span data-ttu-id="70749-109">なし。</span><span class="sxs-lookup"><span data-stu-id="70749-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70749-110">子要素</span><span class="sxs-lookup"><span data-stu-id="70749-110">Child elements</span></span>

<span data-ttu-id="70749-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Discoverysearchconfigurations](discoverysearchconfigurations.md)</span><span class="sxs-lookup"><span data-stu-id="70749-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [DiscoverySearchConfigurations](discoverysearchconfigurations.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70749-112">親要素</span><span class="sxs-lookup"><span data-stu-id="70749-112">Parent elements</span></span>

[<span data-ttu-id="70749-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="70749-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="70749-114">注釈</span><span class="sxs-lookup"><span data-stu-id="70749-114">Remarks</span></span>

<span data-ttu-id="70749-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="70749-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="70749-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="70749-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70749-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="70749-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70749-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="70749-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="70749-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="70749-119">Schema name</span></span>  <br/> |<span data-ttu-id="70749-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="70749-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="70749-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="70749-121">Validation file</span></span>  <br/> |<span data-ttu-id="70749-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="70749-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="70749-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="70749-123">Can be empty</span></span>  <br/> |<span data-ttu-id="70749-124">false</span><span class="sxs-lookup"><span data-stu-id="70749-124">false</span></span>  <br/> |
   

