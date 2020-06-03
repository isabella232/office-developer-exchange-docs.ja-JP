---
title: GetUserSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 832a9211-d2d5-4a49-bcb3-1dc6dc3904ed
description: GetUserSettingsRequest 要素は、1人または複数のユーザーに対して指定された設定を取得する要求を表します。
ms.openlocfilehash: 353facb5d0bbf922a23b33cbaf6f9d2e7d82bd6b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530163"
---
# <a name="getusersettingsrequest-soap"></a><span data-ttu-id="d044a-103">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d044a-103">GetUserSettingsRequest (SOAP)</span></span>

<span data-ttu-id="d044a-104">**Getusersettingsrequest**要素は、1人または複数のユーザーに対して指定された設定を取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="d044a-104">The **GetUserSettingsRequest** element represents a request to retrieve specified settings for one or more users.</span></span> 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
```

 <span data-ttu-id="d044a-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="d044a-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d044a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d044a-106">Attributes and elements</span></span>

<span data-ttu-id="d044a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d044a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d044a-108">属性</span><span class="sxs-lookup"><span data-stu-id="d044a-108">Attributes</span></span>

<span data-ttu-id="d044a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d044a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d044a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d044a-110">Child elements</span></span>

|<span data-ttu-id="d044a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d044a-111">**Element**</span></span>|<span data-ttu-id="d044a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d044a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d044a-113">Users (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d044a-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="d044a-114">設定を取得するユーザーの電子メールアドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="d044a-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="d044a-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d044a-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="d044a-116">要求された構成設定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d044a-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="d044a-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d044a-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="d044a-118">プロバイダーが使用する特定のサーバーのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="d044a-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d044a-119">親要素</span><span class="sxs-lookup"><span data-stu-id="d044a-119">Parent elements</span></span>

<span data-ttu-id="d044a-120">なし。</span><span class="sxs-lookup"><span data-stu-id="d044a-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d044a-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d044a-121">Text value</span></span>

<span data-ttu-id="d044a-122">なし。</span><span class="sxs-lookup"><span data-stu-id="d044a-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d044a-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d044a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d044a-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d044a-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d044a-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d044a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d044a-126">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="d044a-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d044a-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d044a-127">Validation File</span></span>  <br/> |<span data-ttu-id="d044a-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d044a-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d044a-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d044a-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="d044a-130">正しい</span><span class="sxs-lookup"><span data-stu-id="d044a-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d044a-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="d044a-131">See also</span></span>



[<span data-ttu-id="d044a-132">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d044a-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

