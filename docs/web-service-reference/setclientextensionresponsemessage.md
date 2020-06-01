---
title: SetClientExtensionResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3365e58c-adb3-4d92-92cc-acc95ce36cca
description: SetClientExtensionResponseMessage 要素は、SetClientExtension 要求の応答メッセージを指定します。
ms.openlocfilehash: 3743d2f1643bece044ff7b7c8ccac95bbd7401ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468720"
---
# <a name="setclientextensionresponsemessage"></a><span data-ttu-id="d781f-103">SetClientExtensionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d781f-103">SetClientExtensionResponseMessage</span></span>

<span data-ttu-id="d781f-104">**SetClientExtensionResponseMessage**要素は、 **setclientextension**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="d781f-104">The **SetClientExtensionResponseMessage** element specifies the response message for a **SetClientExtension** request.</span></span> 
  
```XML
<SetClientExtensionResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SetClientExtensionResponseMessage>
```

 <span data-ttu-id="d781f-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d781f-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d781f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d781f-106">Attributes and elements</span></span>

<span data-ttu-id="d781f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d781f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d781f-108">属性</span><span class="sxs-lookup"><span data-stu-id="d781f-108">Attributes</span></span>

<span data-ttu-id="d781f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d781f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d781f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d781f-110">Child elements</span></span>

<span data-ttu-id="d781f-111">[Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)  | [MessageXml](messagexml.md)</span><span class="sxs-lookup"><span data-stu-id="d781f-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d781f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d781f-112">Parent elements</span></span>

[<span data-ttu-id="d781f-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d781f-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="d781f-114">注釈</span><span class="sxs-lookup"><span data-stu-id="d781f-114">Remarks</span></span>

<span data-ttu-id="d781f-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d781f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d781f-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d781f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d781f-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d781f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d781f-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="d781f-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d781f-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d781f-119">Schema name</span></span>  <br/> |<span data-ttu-id="d781f-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d781f-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="d781f-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d781f-121">Validation file</span></span>  <br/> |<span data-ttu-id="d781f-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d781f-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d781f-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d781f-123">Can be empty</span></span>  <br/> ||
   

