---
title: UserSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: abb175c5-4f38-4dcc-81e3-b511686862eb
description: UserSettingError 要素は、ユーザー設定を取得しようとした結果として返されるエラーを表します。
ms.openlocfilehash: 61603038ce93780f690d72226b1356b239d2002d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468608"
---
# <a name="usersettingerror-soap"></a><span data-ttu-id="3bdbb-103">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3bdbb-103">UserSettingError (SOAP)</span></span>

<span data-ttu-id="3bdbb-104">**Usersettingerror**要素は、ユーザー設定を取得しようとした結果として返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="3bdbb-104">The **UserSettingError** element represents an error that is returned as a result of an attempt to get a user setting.</span></span> 
  
```XML
<UserSettingError>
    <ErrorCode/>
    <ErrorMessage/>
    <SettingName/>
</UserSettingError>
```

 <span data-ttu-id="3bdbb-105">**UserSettingError**</span><span class="sxs-lookup"><span data-stu-id="3bdbb-105">**UserSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3bdbb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3bdbb-106">Attributes and elements</span></span>

<span data-ttu-id="3bdbb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3bdbb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3bdbb-108">属性</span><span class="sxs-lookup"><span data-stu-id="3bdbb-108">Attributes</span></span>

<span data-ttu-id="3bdbb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3bdbb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3bdbb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3bdbb-110">Child elements</span></span>

|<span data-ttu-id="3bdbb-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="3bdbb-111">**Element**</span></span>|<span data-ttu-id="3bdbb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3bdbb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bdbb-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3bdbb-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="3bdbb-114">自動検出サービスによって返されるエラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="3bdbb-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3bdbb-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3bdbb-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="3bdbb-116">このメッセージは、自動検出サービスによって返されるエラーコードに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="3bdbb-116">Respresents a message associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3bdbb-117">SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3bdbb-117">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="3bdbb-118">ユーザー設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="3bdbb-118">Represents the name of a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3bdbb-119">親要素</span><span class="sxs-lookup"><span data-stu-id="3bdbb-119">Parent elements</span></span>

|<span data-ttu-id="3bdbb-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="3bdbb-120">**Element**</span></span>|<span data-ttu-id="3bdbb-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="3bdbb-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bdbb-122">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3bdbb-122">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="3bdbb-123">返すことができなかった設定に関する情報のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="3bdbb-123">Represents a collection of information about settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3bdbb-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3bdbb-124">Text value</span></span>

<span data-ttu-id="3bdbb-125">なし。</span><span class="sxs-lookup"><span data-stu-id="3bdbb-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3bdbb-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3bdbb-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3bdbb-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="3bdbb-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3bdbb-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3bdbb-128">Schema Name</span></span>  <br/> |<span data-ttu-id="3bdbb-129">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="3bdbb-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3bdbb-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3bdbb-130">Validation File</span></span>  <br/> |<span data-ttu-id="3bdbb-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3bdbb-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3bdbb-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3bdbb-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="3bdbb-133">正しい</span><span class="sxs-lookup"><span data-stu-id="3bdbb-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3bdbb-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="3bdbb-134">See also</span></span>



[<span data-ttu-id="3bdbb-135">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="3bdbb-135">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

