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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459126"
---
# <a name="getumpropertiesresponse-um-web-service"></a><span data-ttu-id="29c5f-103">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="29c5f-103">GetUMPropertiesResponse (UM web service)</span></span>

<span data-ttu-id="29c5f-104">**Getumpropertiesresponse**要素は、 [getumproperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="29c5f-104">The **GetUMPropertiesResponse** element defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="29c5f-105">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="29c5f-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="29c5f-106">**UMProperties**</span><span class="sxs-lookup"><span data-stu-id="29c5f-106">**UMProperties**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29c5f-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="29c5f-107">Attributes and elements</span></span>

<span data-ttu-id="29c5f-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="29c5f-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29c5f-109">属性</span><span class="sxs-lookup"><span data-stu-id="29c5f-109">Attributes</span></span>

<span data-ttu-id="29c5f-110">なし。</span><span class="sxs-lookup"><span data-stu-id="29c5f-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29c5f-111">子要素</span><span class="sxs-lookup"><span data-stu-id="29c5f-111">Child elements</span></span>

|<span data-ttu-id="29c5f-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="29c5f-112">**Element**</span></span>|<span data-ttu-id="29c5f-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="29c5f-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29c5f-114">MissedCallNotificationEnabled (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="29c5f-114">MissedCallNotificationEnabled (UM web service)</span></span>](missedcallnotificationenabled-um-web-service.md) <br/> |<span data-ttu-id="29c5f-115">不在着信通知を有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29c5f-115">Indicates whether missed call notifications are enabled.</span></span>  <br/> |
|[<span data-ttu-id="29c5f-116">PlayOnPhoneDialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="29c5f-116">PlayOnPhoneDialString (UM web service)</span></span>](playonphonedialstring-um-web-service.md) <br/> |<span data-ttu-id="29c5f-117">[Playonphone 操作 (um web サービス)](playonphone-operation-um-web-service.md)および[Playonphone 案内応答操作 (um web サービス)](playonphonegreeting-operation-um-web-service.md)に使用する既定のダイヤル文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="29c5f-117">Contains the default dial string to use for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>  <br/> |
|[<span data-ttu-id="29c5f-118">受付電話番号 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="29c5f-118">TelephoneAccessNumbers (UM web service)</span></span>](telephoneaccessnumbers-um-web-service.md) <br/> |<span data-ttu-id="29c5f-119">ユーザーが電話でユニファイドメッセージングにアクセスする際に使用できる電話番号の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="29c5f-119">Contains the list of telephone numbers the user can use to access Unified Messaging via a telephone.</span></span>  <br/> |
|[<span data-ttu-id="29c5f-120">受付電話 Accessfolderemail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="29c5f-120">TelephoneAccessFolderEmail (UM web service)</span></span>](telephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="29c5f-121">ユニファイドメッセージングが電話でメッセージを読み取る電子メールフォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="29c5f-121">Contains the identifier for the e-mail folder from which Unified Messaging will read messages over the telephone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="29c5f-122">親要素</span><span class="sxs-lookup"><span data-stu-id="29c5f-122">Parent elements</span></span>

<span data-ttu-id="29c5f-123">なし。</span><span class="sxs-lookup"><span data-stu-id="29c5f-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="29c5f-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="29c5f-124">Text value</span></span>

<span data-ttu-id="29c5f-125">なし。</span><span class="sxs-lookup"><span data-stu-id="29c5f-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29c5f-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="29c5f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29c5f-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="29c5f-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="29c5f-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="29c5f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="29c5f-129">メッセージ</span><span class="sxs-lookup"><span data-stu-id="29c5f-129">Messages</span></span>  <br/> |
|<span data-ttu-id="29c5f-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="29c5f-130">Validation File</span></span>  <br/> |<span data-ttu-id="29c5f-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="29c5f-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="29c5f-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="29c5f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="29c5f-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="29c5f-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29c5f-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="29c5f-134">See also</span></span>



[<span data-ttu-id="29c5f-135">GetUMProperties 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="29c5f-135">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)

