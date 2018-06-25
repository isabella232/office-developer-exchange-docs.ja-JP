---
title: SettingName (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8bcb0411-58b0-4e37-b97e-00c07dcbecb1
description: SettingName 要素は、応答の設定の名前を表します。
ms.openlocfilehash: 9bf7c8197693bc6887a99ffcbeb2240e1f4c3b20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833468"
---
# <a name="settingname-soap"></a><span data-ttu-id="2850f-103">SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2850f-103">SettingName (SOAP)</span></span>

<span data-ttu-id="2850f-104">**SettingName**要素は、応答の設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="2850f-104">The **SettingName** element represents the name of a setting in the response.</span></span> 
  
```XML
<SettingName/>
```

 <span data-ttu-id="2850f-105">**string**</span><span class="sxs-lookup"><span data-stu-id="2850f-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2850f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2850f-106">Attributes and elements</span></span>

<span data-ttu-id="2850f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2850f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2850f-108">属性</span><span class="sxs-lookup"><span data-stu-id="2850f-108">Attributes</span></span>

<span data-ttu-id="2850f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2850f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2850f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2850f-110">Child elements</span></span>

<span data-ttu-id="2850f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2850f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2850f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2850f-112">Parent elements</span></span>

|<span data-ttu-id="2850f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="2850f-113">**Element**</span></span>|<span data-ttu-id="2850f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2850f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2850f-115">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2850f-115">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="2850f-116">ユーザー設定の取得中に返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="2850f-116">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="2850f-117">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2850f-117">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="2850f-118">ドメインの設定を取得中に発生したエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="2850f-118">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="2850f-119">これは、 **GetDomainSettings**要求のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="2850f-119">This represents an error from a **GetDomainSettings** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2850f-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2850f-120">Text value</span></span>

<span data-ttu-id="2850f-121">**SettingName**要素の値は、応答の設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="2850f-121">The value of the **SettingName** element represents the name of a setting in a response.</span></span> 
  
<span data-ttu-id="2850f-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2850f-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2850f-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="2850f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2850f-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="2850f-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="2850f-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2850f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2850f-126">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="2850f-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="2850f-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2850f-127">Validation File</span></span>  <br/> |<span data-ttu-id="2850f-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2850f-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2850f-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2850f-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="2850f-130">True</span><span class="sxs-lookup"><span data-stu-id="2850f-130">True</span></span>  <br/> |
   

