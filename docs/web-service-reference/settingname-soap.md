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
ms.openlocfilehash: d492b82b7385d6403f15c08356db5d0503792d54
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466725"
---
# <a name="settingname-soap"></a><span data-ttu-id="37a70-103">SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="37a70-103">SettingName (SOAP)</span></span>

<span data-ttu-id="37a70-104">**Settingname**要素は、応答の設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="37a70-104">The **SettingName** element represents the name of a setting in the response.</span></span> 
  
```XML
<SettingName/>
```

 <span data-ttu-id="37a70-105">**string**</span><span class="sxs-lookup"><span data-stu-id="37a70-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37a70-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="37a70-106">Attributes and elements</span></span>

<span data-ttu-id="37a70-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="37a70-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37a70-108">属性</span><span class="sxs-lookup"><span data-stu-id="37a70-108">Attributes</span></span>

<span data-ttu-id="37a70-109">なし。</span><span class="sxs-lookup"><span data-stu-id="37a70-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37a70-110">子要素</span><span class="sxs-lookup"><span data-stu-id="37a70-110">Child elements</span></span>

<span data-ttu-id="37a70-111">なし。</span><span class="sxs-lookup"><span data-stu-id="37a70-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="37a70-112">親要素</span><span class="sxs-lookup"><span data-stu-id="37a70-112">Parent elements</span></span>

|<span data-ttu-id="37a70-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="37a70-113">**Element**</span></span>|<span data-ttu-id="37a70-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="37a70-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37a70-115">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="37a70-115">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="37a70-116">ユーザー設定の取得中に返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="37a70-116">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="37a70-117">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="37a70-117">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="37a70-118">ドメイン設定の取得中に発生したエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="37a70-118">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="37a70-119">これは、 **Getdomainsettings**要求からのエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="37a70-119">This represents an error from a **GetDomainSettings** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="37a70-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="37a70-120">Text value</span></span>

<span data-ttu-id="37a70-121">**Settingname**要素の値は、応答の設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="37a70-121">The value of the **SettingName** element represents the name of a setting in a response.</span></span> 
  
<span data-ttu-id="37a70-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="37a70-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37a70-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="37a70-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37a70-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="37a70-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="37a70-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="37a70-125">Schema Name</span></span>  <br/> |<span data-ttu-id="37a70-126">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="37a70-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="37a70-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="37a70-127">Validation File</span></span>  <br/> |<span data-ttu-id="37a70-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="37a70-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="37a70-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="37a70-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="37a70-130">はい</span><span class="sxs-lookup"><span data-stu-id="37a70-130">True</span></span>  <br/> |
   

