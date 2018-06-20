---
title: GetDiscoverySearchConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b84a4c6-cb0a-4bca-85b2-fec32227930b
description: GetDiscoverySearchConfigurationResponseMessage 要素は、GetDiscoverySearchConfiguration 要求の応答メッセージを指定します。
ms.openlocfilehash: a6cf09753031a7fd2eb46132e8bfb0729140d6c3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760693"
---
# <a name="getdiscoverysearchconfigurationresponsemessage"></a><span data-ttu-id="91cce-103">GetDiscoverySearchConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="91cce-103">GetDiscoverySearchConfigurationResponseMessage</span></span>

<span data-ttu-id="91cce-104">**GetDiscoverySearchConfigurationResponseMessage**要素は、 **GetDiscoverySearchConfiguration**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="91cce-104">The **GetDiscoverySearchConfigurationResponseMessage** element specifies the response message for a **GetDiscoverySearchConfiguration** request.</span></span> 
  
```XML
<GetDiscoverySearchConfigurationResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DiscoverySearchConfigurations/>
</GetDiscoverySearchConfigurationResponseMessage>
```

 <span data-ttu-id="91cce-105">**GetDiscoverySearchConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="91cce-105">**GetDiscoverySearchConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91cce-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="91cce-106">Attributes and elements</span></span>

<span data-ttu-id="91cce-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="91cce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91cce-108">属性</span><span class="sxs-lookup"><span data-stu-id="91cce-108">Attributes</span></span>

<span data-ttu-id="91cce-109">なし。</span><span class="sxs-lookup"><span data-stu-id="91cce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91cce-110">子要素</span><span class="sxs-lookup"><span data-stu-id="91cce-110">Child elements</span></span>

<span data-ttu-id="91cce-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [DiscoverySearchConfigurations](discoverysearchconfigurations.md)</span><span class="sxs-lookup"><span data-stu-id="91cce-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [DiscoverySearchConfigurations](discoverysearchconfigurations.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91cce-112">親要素</span><span class="sxs-lookup"><span data-stu-id="91cce-112">Parent elements</span></span>

[<span data-ttu-id="91cce-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="91cce-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="91cce-114">備考</span><span class="sxs-lookup"><span data-stu-id="91cce-114">Remarks</span></span>

<span data-ttu-id="91cce-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="91cce-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="91cce-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="91cce-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91cce-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="91cce-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91cce-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="91cce-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="91cce-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="91cce-119">Schema name</span></span>  <br/> |<span data-ttu-id="91cce-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="91cce-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="91cce-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="91cce-121">Validation file</span></span>  <br/> |<span data-ttu-id="91cce-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="91cce-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="91cce-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="91cce-123">Can be empty</span></span>  <br/> |<span data-ttu-id="91cce-124">false</span><span class="sxs-lookup"><span data-stu-id="91cce-124">false</span></span>  <br/> |
   

