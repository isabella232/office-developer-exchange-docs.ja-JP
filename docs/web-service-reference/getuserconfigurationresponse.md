---
title: GetUserConfigurationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfigurationResponse
api_type:
- schema
ms.assetid: 5e418c91-c836-4de0-a80d-f0dad0c684d7
description: GetUserConfigurationResponse 要素は、単一の GetUserConfiguration 要求に対する応答を定義します。
ms.openlocfilehash: d80f281f8dc02f911281959b8629b0d8908f4e97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457705"
---
# <a name="getuserconfigurationresponse"></a><span data-ttu-id="3b0f7-103">GetUserConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="3b0f7-103">GetUserConfigurationResponse</span></span>

<span data-ttu-id="3b0f7-104">**Getuserconfigurationresponse**要素は、単一の getuserconfiguration 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="3b0f7-104">The **GetUserConfigurationResponse** element defines a response to a single GetUserConfiguration request.</span></span> 
  
```xml
<GetUserConfigurationResponse>   <ResponseMessages/></GetUserConfigurationResponse>
```

 <span data-ttu-id="3b0f7-105">**GetUserConfigurationResponseType**</span><span class="sxs-lookup"><span data-stu-id="3b0f7-105">**GetUserConfigurationResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b0f7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3b0f7-106">Attributes and elements</span></span>

<span data-ttu-id="3b0f7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3b0f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b0f7-108">属性</span><span class="sxs-lookup"><span data-stu-id="3b0f7-108">Attributes</span></span>

<span data-ttu-id="3b0f7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3b0f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b0f7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3b0f7-110">Child elements</span></span>

|<span data-ttu-id="3b0f7-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="3b0f7-111">**Element**</span></span>|<span data-ttu-id="3b0f7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3b0f7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b0f7-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3b0f7-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="3b0f7-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="3b0f7-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3b0f7-115">親要素</span><span class="sxs-lookup"><span data-stu-id="3b0f7-115">Parent elements</span></span>

<span data-ttu-id="3b0f7-116">なし。</span><span class="sxs-lookup"><span data-stu-id="3b0f7-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3b0f7-117">注釈</span><span class="sxs-lookup"><span data-stu-id="3b0f7-117">Remarks</span></span>

<span data-ttu-id="3b0f7-118">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="3b0f7-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b0f7-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3b0f7-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b0f7-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="3b0f7-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3b0f7-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3b0f7-121">Schema Name</span></span>  <br/> |<span data-ttu-id="3b0f7-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3b0f7-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3b0f7-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3b0f7-123">Validation File</span></span>  <br/> |<span data-ttu-id="3b0f7-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3b0f7-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3b0f7-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3b0f7-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b0f7-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="3b0f7-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b0f7-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="3b0f7-127">See also</span></span>



- [<span data-ttu-id="3b0f7-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3b0f7-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

