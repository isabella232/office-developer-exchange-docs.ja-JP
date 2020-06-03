---
title: マニフェスト
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 650d9fc0-1504-4db4-95d6-d3ba86df66ca
description: Manifest 要素には、電子メールアカウント用にインストールされている、base64 でエンコードされたアプリのマニフェストのコレクションが含まれています。
ms.openlocfilehash: 91239e2337f7a1886d8947f558a86110755a93df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44450817"
---
# <a name="manifests"></a><span data-ttu-id="e9400-103">マニフェスト</span><span class="sxs-lookup"><span data-stu-id="e9400-103">Manifests</span></span>

<span data-ttu-id="e9400-104">**Manifest**要素には、電子メールアカウント用にインストールされている、base64 でエンコードされたアプリのマニフェストのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9400-104">The **Manifests** element contains a collection of base64-encoded app manifests that are installed for the email account.</span></span> 
  
```XML
<Manifests>
   <Manifest/>
</Manifests>
```

 <span data-ttu-id="e9400-105">**ArrayOfAppManifestsType**</span><span class="sxs-lookup"><span data-stu-id="e9400-105">**ArrayOfAppManifestsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9400-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e9400-106">Attributes and elements</span></span>

<span data-ttu-id="e9400-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9400-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9400-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9400-108">Attributes</span></span>

<span data-ttu-id="e9400-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e9400-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9400-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e9400-110">Child elements</span></span>

[<span data-ttu-id="e9400-111">マニフェスト</span><span class="sxs-lookup"><span data-stu-id="e9400-111">Manifest</span></span>](manifest.md)
  
### <a name="parent-elements"></a><span data-ttu-id="e9400-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e9400-112">Parent elements</span></span>

[<span data-ttu-id="e9400-113">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="e9400-113">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="e9400-114">注釈</span><span class="sxs-lookup"><span data-stu-id="e9400-114">Remarks</span></span>

<span data-ttu-id="e9400-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e9400-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e9400-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e9400-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9400-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e9400-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9400-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9400-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e9400-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9400-119">Schema name</span></span>  <br/> |<span data-ttu-id="e9400-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="e9400-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e9400-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9400-121">Validation file</span></span>  <br/> |<span data-ttu-id="e9400-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="e9400-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e9400-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e9400-123">Can be empty</span></span>  <br/> ||
   

