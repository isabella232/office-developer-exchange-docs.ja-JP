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
description: GetUMPropertiesResponse 要素は、GetUMProperties の操作 (UM web サービス) 要求に対する応答を定義します。
ms.openlocfilehash: c0df872ad6b8e6541fa750ab87f4c1e5f0118b00
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831685"
---
# <a name="getumpropertiesresponse-um-web-service"></a><span data-ttu-id="48ee2-103">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="48ee2-103">GetUMPropertiesResponse (UM web service)</span></span>

<span data-ttu-id="48ee2-104">**GetUMPropertiesResponse**要素は、 [GetUMProperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="48ee2-104">The **GetUMPropertiesResponse** element defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="48ee2-105">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="48ee2-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="48ee2-106">**UMProperties**</span><span class="sxs-lookup"><span data-stu-id="48ee2-106">**UMProperties**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="48ee2-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="48ee2-107">Attributes and elements</span></span>

<span data-ttu-id="48ee2-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="48ee2-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48ee2-109">属性</span><span class="sxs-lookup"><span data-stu-id="48ee2-109">Attributes</span></span>

<span data-ttu-id="48ee2-110">なし。</span><span class="sxs-lookup"><span data-stu-id="48ee2-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="48ee2-111">子要素</span><span class="sxs-lookup"><span data-stu-id="48ee2-111">Child elements</span></span>

|<span data-ttu-id="48ee2-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="48ee2-112">**Element**</span></span>|<span data-ttu-id="48ee2-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="48ee2-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48ee2-114">MissedCallNotificationEnabled (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="48ee2-114">MissedCallNotificationEnabled (UM web service)</span></span>](missedcallnotificationenabled-um-web-service.md) <br/> |<span data-ttu-id="48ee2-115">不在着信通知が有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="48ee2-115">Indicates whether missed call notifications are enabled.</span></span>  <br/> |
|[<span data-ttu-id="48ee2-116">PlayOnPhoneDialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="48ee2-116">PlayOnPhoneDialString (UM web service)</span></span>](playonphonedialstring-um-web-service.md) <br/> |<span data-ttu-id="48ee2-117">[PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)と[PlayOnPhoneGreeting (UM web サービス) の操作](playonphonegreeting-operation-um-web-service.md)に使用する既定のダイヤル文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="48ee2-117">Contains the default dial string to use for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>  <br/> |
|[<span data-ttu-id="48ee2-118">TelephoneAccessNumbers (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="48ee2-118">TelephoneAccessNumbers (UM web service)</span></span>](telephoneaccessnumbers-um-web-service.md) <br/> |<span data-ttu-id="48ee2-119">電話を使用してユニファイド メッセージングにアクセスするユーザーが使用できる電話番号の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="48ee2-119">Contains the list of telephone numbers the user can use to access Unified Messaging via a telephone.</span></span>  <br/> |
|[<span data-ttu-id="48ee2-120">TelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="48ee2-120">TelephoneAccessFolderEmail (UM web service)</span></span>](telephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="48ee2-121">ユニファイド メッセージングはの読み取り元のメッセージに電話、電子メール フォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="48ee2-121">Contains the identifier for the e-mail folder from which Unified Messaging will read messages over the telephone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="48ee2-122">親要素</span><span class="sxs-lookup"><span data-stu-id="48ee2-122">Parent elements</span></span>

<span data-ttu-id="48ee2-123">なし。</span><span class="sxs-lookup"><span data-stu-id="48ee2-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="48ee2-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="48ee2-124">Text value</span></span>

<span data-ttu-id="48ee2-125">なし。</span><span class="sxs-lookup"><span data-stu-id="48ee2-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="48ee2-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="48ee2-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48ee2-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="48ee2-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="48ee2-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="48ee2-128">Schema Name</span></span>  <br/> |<span data-ttu-id="48ee2-129">メッセージ</span><span class="sxs-lookup"><span data-stu-id="48ee2-129">Messages</span></span>  <br/> |
|<span data-ttu-id="48ee2-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="48ee2-130">Validation File</span></span>  <br/> |<span data-ttu-id="48ee2-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="48ee2-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="48ee2-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="48ee2-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="48ee2-133">False</span><span class="sxs-lookup"><span data-stu-id="48ee2-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="48ee2-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="48ee2-134">See also</span></span>



[<span data-ttu-id="48ee2-135">GetUMProperties 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="48ee2-135">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)

