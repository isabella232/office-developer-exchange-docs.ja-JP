---
title: GetClientExtensionResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ef4b1aba-a55d-4d64-ac80-5d4e6c4e72bd
description: GetClientExtensionResponse 要素には、アプリケーションに関する構成情報を取得する応答が含まれています。
ms.openlocfilehash: 523a103ec9397b0dce08aa47b074303c9e6ac897
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760658"
---
# <a name="getclientextensionresponse"></a><span data-ttu-id="e8b6c-103">GetClientExtensionResponse</span><span class="sxs-lookup"><span data-stu-id="e8b6c-103">GetClientExtensionResponse</span></span>

<span data-ttu-id="e8b6c-104">**GetClientExtensionResponse**要素には、アプリケーションに関する構成情報を取得する応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8b6c-104">The **GetClientExtensionResponse** element contains the response to get configuration information about an app.</span></span> 
  
```XML
<GetClientExtensionResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ClientExtensions/>
   <RawMasterTableXml/>
</GetClientExtensionResponse>
```

 <span data-ttu-id="e8b6c-105">**ClientExtensionResponseType**</span><span class="sxs-lookup"><span data-stu-id="e8b6c-105">**ClientExtensionResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8b6c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e8b6c-106">Attributes and elements</span></span>

<span data-ttu-id="e8b6c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e8b6c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8b6c-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8b6c-108">Attributes</span></span>

<span data-ttu-id="e8b6c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e8b6c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8b6c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e8b6c-110">Child elements</span></span>

<span data-ttu-id="e8b6c-111">[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ClientExtensions](clientextensions.md) | [RawMasterTableXml](rawmastertablexml.md)</span><span class="sxs-lookup"><span data-stu-id="e8b6c-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ClientExtensions](clientextensions.md) | [RawMasterTableXml](rawmastertablexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e8b6c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e8b6c-112">Parent elements</span></span>

<span data-ttu-id="e8b6c-113">なし。</span><span class="sxs-lookup"><span data-stu-id="e8b6c-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8b6c-114">備考</span><span class="sxs-lookup"><span data-stu-id="e8b6c-114">Remarks</span></span>

<span data-ttu-id="e8b6c-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e8b6c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e8b6c-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e8b6c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8b6c-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="e8b6c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8b6c-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="e8b6c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e8b6c-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e8b6c-119">Schema name</span></span>  <br/> |<span data-ttu-id="e8b6c-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e8b6c-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e8b6c-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e8b6c-121">Validation file</span></span>  <br/> |<span data-ttu-id="e8b6c-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e8b6c-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e8b6c-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e8b6c-123">Can be empty</span></span>  <br/> |<span data-ttu-id="e8b6c-124">false</span><span class="sxs-lookup"><span data-stu-id="e8b6c-124">false</span></span>  <br/> |
   

