---
title: GetClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c96c2b4c-45cb-482a-a3bb-7a11a0fff43b
description: GetClientExtension 要素は、クライアント拡張機能を取得する要求を表します。
ms.openlocfilehash: caa069195a3b82af4e5b5984dcb6e4124b11899b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526341"
---
# <a name="getclientextension"></a><span data-ttu-id="77540-103">GetClientExtension</span><span class="sxs-lookup"><span data-stu-id="77540-103">GetClientExtension</span></span>

<span data-ttu-id="77540-104">**Getclientextension**要素は、クライアント拡張機能を取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="77540-104">The **GetClientExtension** element represents a request to get a client extension.</span></span> 
  
```XML
<GetClientExtension>
   <RequestedExtensionIds/>
   <UserParameters/>
   <IsDebug/>
</GetClientExtension>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="77540-105">属性と要素</span><span class="sxs-lookup"><span data-stu-id="77540-105">Attributes and elements</span></span>

<span data-ttu-id="77540-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="77540-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77540-107">属性</span><span class="sxs-lookup"><span data-stu-id="77540-107">Attributes</span></span>

<span data-ttu-id="77540-108">なし。</span><span class="sxs-lookup"><span data-stu-id="77540-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77540-109">子要素</span><span class="sxs-lookup"><span data-stu-id="77540-109">Child elements</span></span>

<span data-ttu-id="77540-110">[RequestedExtensionIds](requestedextensionids.md)  | [Userparameters](userparameters.md)  | [Isdebug](isdebug.md)</span><span class="sxs-lookup"><span data-stu-id="77540-110">[RequestedExtensionIds](requestedextensionids.md) | [UserParameters](userparameters.md) | [IsDebug](isdebug.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="77540-111">親要素</span><span class="sxs-lookup"><span data-stu-id="77540-111">Parent elements</span></span>

<span data-ttu-id="77540-112">なし。</span><span class="sxs-lookup"><span data-stu-id="77540-112">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="77540-113">注釈</span><span class="sxs-lookup"><span data-stu-id="77540-113">Remarks</span></span>

<span data-ttu-id="77540-114">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="77540-114">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="77540-115">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="77540-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77540-116">要素の情報</span><span class="sxs-lookup"><span data-stu-id="77540-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77540-117">Namespace</span><span class="sxs-lookup"><span data-stu-id="77540-117">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="77540-118">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="77540-118">Schema name</span></span>  <br/> |<span data-ttu-id="77540-119">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="77540-119">Messages schema</span></span>  <br/> |
|<span data-ttu-id="77540-120">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="77540-120">Validation file</span></span>  <br/> |<span data-ttu-id="77540-121">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="77540-121">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="77540-122">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="77540-122">Can be empty</span></span>  <br/> ||
   

