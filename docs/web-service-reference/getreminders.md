---
title: GetReminders
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 943c3d5d-7d29-4d70-932c-8a4fe44a0037
description: GetReminders 要素は、事前通知を取得する要求を指定します。
ms.openlocfilehash: f4ecc858af2150bb3f88ebdf9ed541892f2fead1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760840"
---
# <a name="getreminders"></a><span data-ttu-id="669c7-103">GetReminders</span><span class="sxs-lookup"><span data-stu-id="669c7-103">GetReminders</span></span>

<span data-ttu-id="669c7-104">**GetReminders**要素は、事前通知を取得する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="669c7-104">The **GetReminders** element specifies a request to get reminders.</span></span> 
  
```XML
<GetReminders>
   <BeginTime/>
   <EndTime/>
   <MaxItems/>
   <ReminderType/>
</GetReminders>

```

 <span data-ttu-id="669c7-105">**GetRemindersType**</span><span class="sxs-lookup"><span data-stu-id="669c7-105">**GetRemindersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="669c7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="669c7-106">Attributes and elements</span></span>

<span data-ttu-id="669c7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="669c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="669c7-108">属性</span><span class="sxs-lookup"><span data-stu-id="669c7-108">Attributes</span></span>

<span data-ttu-id="669c7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="669c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="669c7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="669c7-110">Child elements</span></span>

<span data-ttu-id="669c7-111">[BeginTime](begintime.md) | [終了時刻 (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [MaxItems](maxitems.md) | [ReminderType](remindertype.md)</span><span class="sxs-lookup"><span data-stu-id="669c7-111">[BeginTime](begintime.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [MaxItems](maxitems.md) | [ReminderType](remindertype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="669c7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="669c7-112">Parent elements</span></span>

<span data-ttu-id="669c7-113">なし。</span><span class="sxs-lookup"><span data-stu-id="669c7-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="669c7-114">解説</span><span class="sxs-lookup"><span data-stu-id="669c7-114">Remarks</span></span>

<span data-ttu-id="669c7-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="669c7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="669c7-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="669c7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="669c7-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="669c7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="669c7-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="669c7-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="669c7-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="669c7-119">Schema Name</span></span>  <br/> |<span data-ttu-id="669c7-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="669c7-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="669c7-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="669c7-121">Validation File</span></span>  <br/> |<span data-ttu-id="669c7-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="669c7-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="669c7-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="669c7-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="669c7-124">True</span><span class="sxs-lookup"><span data-stu-id="669c7-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="669c7-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="669c7-125">See also</span></span>



- [<span data-ttu-id="669c7-126">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="669c7-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

