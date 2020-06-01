---
title: GetClientExtensionResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ef4b1aba-a55d-4d64-ac80-5d4e6c4e72bd
description: GetClientExtensionResponse 要素は、アプリに関する構成情報を取得するための応答を含みます。
ms.openlocfilehash: 65c1995fe75b3894607d27ed65548fbbdce0664a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459519"
---
# <a name="getclientextensionresponse"></a><span data-ttu-id="33962-103">GetClientExtensionResponse</span><span class="sxs-lookup"><span data-stu-id="33962-103">GetClientExtensionResponse</span></span>

<span data-ttu-id="33962-104">**Getclientextensionresponse**要素は、アプリに関する構成情報を取得するための応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="33962-104">The **GetClientExtensionResponse** element contains the response to get configuration information about an app.</span></span> 
  
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

 <span data-ttu-id="33962-105">**ClientExtensionResponseType**</span><span class="sxs-lookup"><span data-stu-id="33962-105">**ClientExtensionResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33962-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="33962-106">Attributes and elements</span></span>

<span data-ttu-id="33962-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="33962-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33962-108">属性</span><span class="sxs-lookup"><span data-stu-id="33962-108">Attributes</span></span>

<span data-ttu-id="33962-109">なし。</span><span class="sxs-lookup"><span data-stu-id="33962-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33962-110">子要素</span><span class="sxs-lookup"><span data-stu-id="33962-110">Child elements</span></span>

<span data-ttu-id="33962-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)  | [Clientextensions](clientextensions.md)  | [RawMasterTableXml](rawmastertablexml.md)</span><span class="sxs-lookup"><span data-stu-id="33962-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ClientExtensions](clientextensions.md) | [RawMasterTableXml](rawmastertablexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33962-112">親要素</span><span class="sxs-lookup"><span data-stu-id="33962-112">Parent elements</span></span>

<span data-ttu-id="33962-113">なし。</span><span class="sxs-lookup"><span data-stu-id="33962-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="33962-114">注釈</span><span class="sxs-lookup"><span data-stu-id="33962-114">Remarks</span></span>

<span data-ttu-id="33962-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="33962-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="33962-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="33962-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33962-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="33962-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33962-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="33962-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="33962-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="33962-119">Schema name</span></span>  <br/> |<span data-ttu-id="33962-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="33962-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="33962-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="33962-121">Validation file</span></span>  <br/> |<span data-ttu-id="33962-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="33962-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33962-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="33962-123">Can be empty</span></span>  <br/> |<span data-ttu-id="33962-124">false</span><span class="sxs-lookup"><span data-stu-id="33962-124">false</span></span>  <br/> |
   

