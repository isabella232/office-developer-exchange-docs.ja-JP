---
title: ConfigurationRequestDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 545cfe9d-9995-44d6-a3d0-4d43a169cf67
description: ConfigurationRequestDetails 要素には、微調整するポリシーのクライアントの状態が含まれています。 状態情報には、インストールされているルールとクライアント コンポーネントのバージョンを含めることができます。
ms.openlocfilehash: 5195f32f6711ad565922918893209dc01d68d7c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759655"
---
# <a name="configurationrequestdetails"></a><span data-ttu-id="a4212-104">ConfigurationRequestDetails</span><span class="sxs-lookup"><span data-stu-id="a4212-104">ConfigurationRequestDetails</span></span>

<span data-ttu-id="a4212-105">**ConfigurationRequestDetails**要素には、微調整するポリシーのクライアントの状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a4212-105">The **ConfigurationRequestDetails** element contains client state for policy nudges.</span></span> <span data-ttu-id="a4212-106">状態情報には、インストールされているルールとクライアント コンポーネントのバージョンを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a4212-106">State information can include the rules that are installed and client component version.</span></span> 
  
```XML
<ConfigurationRequestDetails></ConfigurationRequestDetails>
```

 <span data-ttu-id="a4212-107">**ConfigurationRequestDetailsType**</span><span class="sxs-lookup"><span data-stu-id="a4212-107">**ConfigurationRequestDetailsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4212-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a4212-108">Attributes and elements</span></span>

<span data-ttu-id="a4212-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a4212-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4212-110">属性</span><span class="sxs-lookup"><span data-stu-id="a4212-110">Attributes</span></span>

<span data-ttu-id="a4212-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a4212-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4212-112">子要素</span><span class="sxs-lookup"><span data-stu-id="a4212-112">Child elements</span></span>

<span data-ttu-id="a4212-113">子要素は、Exchange Web サービスのスキーマで定義されていません。</span><span class="sxs-lookup"><span data-stu-id="a4212-113">The child elements are not defined in the Exchange Web Services schema.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a4212-114">親要素</span><span class="sxs-lookup"><span data-stu-id="a4212-114">Parent elements</span></span>

[<span data-ttu-id="a4212-115">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4212-115">GetServiceConfiguration</span></span>](getserviceconfiguration.md)
  
## <a name="remarks"></a><span data-ttu-id="a4212-116">備考</span><span class="sxs-lookup"><span data-stu-id="a4212-116">Remarks</span></span>

<span data-ttu-id="a4212-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a4212-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a4212-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a4212-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4212-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="a4212-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4212-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="a4212-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a4212-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a4212-121">Schema name</span></span>  <br/> |<span data-ttu-id="a4212-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a4212-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a4212-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a4212-123">Validation file</span></span>  <br/> |<span data-ttu-id="a4212-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a4212-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a4212-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a4212-125">Can be empty</span></span>  <br/> |<span data-ttu-id="a4212-126">false</span><span class="sxs-lookup"><span data-stu-id="a4212-126">false</span></span>  <br/> |
   

