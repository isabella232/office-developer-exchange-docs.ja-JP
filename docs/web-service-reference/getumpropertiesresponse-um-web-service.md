---
title: GetUMPropertiesResponse (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMPropertiesResponse
api_type:
- schema
ms.assetid: fcd93ce5-7403-46a9-b46e-56d2ebdd2f79
description: GetUMPropertiesResponse 要素は、GetUMProperties 操作 (UM web サービス) 要求への応答を定義します。
ms.openlocfilehash: 3247489a305c694c10764d7a0c6f02b1fad51ebf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459126"
---
# <a name="getumpropertiesresponse-um-web-service"></a><span data-ttu-id="76e19-103">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="76e19-103">GetUMPropertiesResponse (UM web service)</span></span>

<span data-ttu-id="76e19-104">**Getumpropertiesresponse**要素は、 [getumproperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="76e19-104">The **GetUMPropertiesResponse** element defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="76e19-105">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="76e19-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="76e19-106">**UMProperties**</span><span class="sxs-lookup"><span data-stu-id="76e19-106">**UMProperties**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76e19-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="76e19-107">Attributes and elements</span></span>

<span data-ttu-id="76e19-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="76e19-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76e19-109">属性</span><span class="sxs-lookup"><span data-stu-id="76e19-109">Attributes</span></span>

<span data-ttu-id="76e19-110">なし。</span><span class="sxs-lookup"><span data-stu-id="76e19-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76e19-111">子要素</span><span class="sxs-lookup"><span data-stu-id="76e19-111">Child elements</span></span>

|<span data-ttu-id="76e19-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="76e19-112">**Element**</span></span>|<span data-ttu-id="76e19-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="76e19-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76e19-114">MissedCallNotificationEnabled (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="76e19-114">MissedCallNotificationEnabled (UM web service)</span></span>](missedcallnotificationenabled-um-web-service.md) <br/> |<span data-ttu-id="76e19-115">不在着信通知を有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="76e19-115">Indicates whether missed call notifications are enabled.</span></span>  <br/> |
|[<span data-ttu-id="76e19-116">PlayOnPhoneDialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="76e19-116">PlayOnPhoneDialString (UM web service)</span></span>](playonphonedialstring-um-web-service.md) <br/> |<span data-ttu-id="76e19-117">[Playonphone 操作 (um web サービス)](playonphone-operation-um-web-service.md)および[Playonphone 案内応答操作 (um web サービス)](playonphonegreeting-operation-um-web-service.md)に使用する既定のダイヤル文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76e19-117">Contains the default dial string to use for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>  <br/> |
|[<span data-ttu-id="76e19-118">受付電話番号 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="76e19-118">TelephoneAccessNumbers (UM web service)</span></span>](telephoneaccessnumbers-um-web-service.md) <br/> |<span data-ttu-id="76e19-119">ユーザーが電話でユニファイドメッセージングにアクセスする際に使用できる電話番号の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76e19-119">Contains the list of telephone numbers the user can use to access Unified Messaging via a telephone.</span></span>  <br/> |
|[<span data-ttu-id="76e19-120">受付電話 Accessfolderemail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="76e19-120">TelephoneAccessFolderEmail (UM web service)</span></span>](telephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="76e19-121">ユニファイドメッセージングが電話でメッセージを読み取る電子メールフォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76e19-121">Contains the identifier for the e-mail folder from which Unified Messaging will read messages over the telephone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76e19-122">親要素</span><span class="sxs-lookup"><span data-stu-id="76e19-122">Parent elements</span></span>

<span data-ttu-id="76e19-123">なし。</span><span class="sxs-lookup"><span data-stu-id="76e19-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="76e19-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="76e19-124">Text value</span></span>

<span data-ttu-id="76e19-125">なし。</span><span class="sxs-lookup"><span data-stu-id="76e19-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76e19-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="76e19-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76e19-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="76e19-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="76e19-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="76e19-128">Schema Name</span></span>  <br/> |<span data-ttu-id="76e19-129">メッセージ</span><span class="sxs-lookup"><span data-stu-id="76e19-129">Messages</span></span>  <br/> |
|<span data-ttu-id="76e19-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="76e19-130">Validation File</span></span>  <br/> |<span data-ttu-id="76e19-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="76e19-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="76e19-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="76e19-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="76e19-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="76e19-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76e19-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="76e19-134">See also</span></span>



[<span data-ttu-id="76e19-135">GetUMProperties 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="76e19-135">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)

