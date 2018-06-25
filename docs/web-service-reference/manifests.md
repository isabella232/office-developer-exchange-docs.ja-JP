---
title: マニフェスト
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 650d9fc0-1504-4db4-95d6-d3ba86df66ca
description: マニフェストの要素には、電子メール アカウントにインストールされている base64 でエンコードされたアプリケーション マニフェストのコレクションが含まれています。
ms.openlocfilehash: 3877841c097e6b968d0af51ae5261e5b4336c7ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832362"
---
# <a name="manifests"></a><span data-ttu-id="def64-103">マニフェスト</span><span class="sxs-lookup"><span data-stu-id="def64-103">Manifests</span></span>

<span data-ttu-id="def64-104">**マニフェスト**の要素には、電子メール アカウントにインストールされている base64 でエンコードされたアプリケーション マニフェストのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="def64-104">The **Manifests** element contains a collection of base64-encoded app manifests that are installed for the email account.</span></span> 
  
```XML
<Manifests>
   <Manifest/>
</Manifests>
```

 <span data-ttu-id="def64-105">**ArrayOfAppManifestsType**</span><span class="sxs-lookup"><span data-stu-id="def64-105">**ArrayOfAppManifestsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="def64-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="def64-106">Attributes and elements</span></span>

<span data-ttu-id="def64-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="def64-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="def64-108">属性</span><span class="sxs-lookup"><span data-stu-id="def64-108">Attributes</span></span>

<span data-ttu-id="def64-109">なし。</span><span class="sxs-lookup"><span data-stu-id="def64-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="def64-110">子要素</span><span class="sxs-lookup"><span data-stu-id="def64-110">Child elements</span></span>

[<span data-ttu-id="def64-111">Manifest</span><span class="sxs-lookup"><span data-stu-id="def64-111">Manifest</span></span>](manifest.md)
  
### <a name="parent-elements"></a><span data-ttu-id="def64-112">親要素</span><span class="sxs-lookup"><span data-stu-id="def64-112">Parent elements</span></span>

[<span data-ttu-id="def64-113">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="def64-113">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="def64-114">備考</span><span class="sxs-lookup"><span data-stu-id="def64-114">Remarks</span></span>

<span data-ttu-id="def64-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="def64-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="def64-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="def64-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="def64-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="def64-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="def64-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="def64-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="def64-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="def64-119">Schema name</span></span>  <br/> |<span data-ttu-id="def64-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="def64-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="def64-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="def64-121">Validation file</span></span>  <br/> |<span data-ttu-id="def64-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="def64-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="def64-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="def64-123">Can be empty</span></span>  <br/> ||
   

