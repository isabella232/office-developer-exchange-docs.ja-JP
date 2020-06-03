---
title: ConfigurationRequestDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 545cfe9d-9995-44d6-a3d0-4d43a169cf67
description: ConfigurationRequestDetails 要素には、ポリシーシェイクのクライアントの状態が含まれています。 状態情報には、インストールされているルールとクライアントコンポーネントのバージョンを含めることができます。
ms.openlocfilehash: 302327a13a108f1d87d39bdfd16346a6c43a7557
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463917"
---
# <a name="configurationrequestdetails"></a><span data-ttu-id="f4f39-104">ConfigurationRequestDetails</span><span class="sxs-lookup"><span data-stu-id="f4f39-104">ConfigurationRequestDetails</span></span>

<span data-ttu-id="f4f39-105">**Configurationrequestdetails**要素には、ポリシーシェイクのクライアントの状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f4f39-105">The **ConfigurationRequestDetails** element contains client state for policy nudges.</span></span> <span data-ttu-id="f4f39-106">状態情報には、インストールされているルールとクライアントコンポーネントのバージョンを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f4f39-106">State information can include the rules that are installed and client component version.</span></span> 
  
```XML
<ConfigurationRequestDetails></ConfigurationRequestDetails>
```

 <span data-ttu-id="f4f39-107">**Configurationrequest/Stype**</span><span class="sxs-lookup"><span data-stu-id="f4f39-107">**ConfigurationRequestDetailsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4f39-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f4f39-108">Attributes and elements</span></span>

<span data-ttu-id="f4f39-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f4f39-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4f39-110">属性</span><span class="sxs-lookup"><span data-stu-id="f4f39-110">Attributes</span></span>

<span data-ttu-id="f4f39-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f4f39-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4f39-112">子要素</span><span class="sxs-lookup"><span data-stu-id="f4f39-112">Child elements</span></span>

<span data-ttu-id="f4f39-113">子要素は、Exchange Web サービススキーマでは定義されていません。</span><span class="sxs-lookup"><span data-stu-id="f4f39-113">The child elements are not defined in the Exchange Web Services schema.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f4f39-114">親要素</span><span class="sxs-lookup"><span data-stu-id="f4f39-114">Parent elements</span></span>

[<span data-ttu-id="f4f39-115">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4f39-115">GetServiceConfiguration</span></span>](getserviceconfiguration.md)
  
## <a name="remarks"></a><span data-ttu-id="f4f39-116">注釈</span><span class="sxs-lookup"><span data-stu-id="f4f39-116">Remarks</span></span>

<span data-ttu-id="f4f39-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f4f39-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f4f39-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f4f39-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4f39-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f4f39-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4f39-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="f4f39-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f4f39-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f4f39-121">Schema name</span></span>  <br/> |<span data-ttu-id="f4f39-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f4f39-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f4f39-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f4f39-123">Validation file</span></span>  <br/> |<span data-ttu-id="f4f39-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f4f39-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f4f39-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f4f39-125">Can be empty</span></span>  <br/> |<span data-ttu-id="f4f39-126">false</span><span class="sxs-lookup"><span data-stu-id="f4f39-126">false</span></span>  <br/> |
   

