---
title: GetReminders
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 943c3d5d-7d29-4d70-932c-8a4fe44a0037
description: GetReminders 要素は、アラームを取得する要求を指定します。
ms.openlocfilehash: 8b869730f39876b838fbcbef3c39661238ed203c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458300"
---
# <a name="getreminders"></a><span data-ttu-id="7d6bb-103">GetReminders</span><span class="sxs-lookup"><span data-stu-id="7d6bb-103">GetReminders</span></span>

<span data-ttu-id="7d6bb-104">**Getreminders**要素は、アラームを取得する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d6bb-104">The **GetReminders** element specifies a request to get reminders.</span></span> 
  
```XML
<GetReminders>
   <BeginTime/>
   <EndTime/>
   <MaxItems/>
   <ReminderType/>
</GetReminders>

```

 <span data-ttu-id="7d6bb-105">**GetRemindersType**</span><span class="sxs-lookup"><span data-stu-id="7d6bb-105">**GetRemindersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d6bb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7d6bb-106">Attributes and elements</span></span>

<span data-ttu-id="7d6bb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7d6bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d6bb-108">属性</span><span class="sxs-lookup"><span data-stu-id="7d6bb-108">Attributes</span></span>

<span data-ttu-id="7d6bb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7d6bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d6bb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7d6bb-110">Child elements</span></span>

<span data-ttu-id="7d6bb-111">[Begintime](begintime.md)  | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md)  | [MaxItems](maxitems.md)  | [ReminderType](remindertype.md)</span><span class="sxs-lookup"><span data-stu-id="7d6bb-111">[BeginTime](begintime.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [MaxItems](maxitems.md) | [ReminderType](remindertype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7d6bb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7d6bb-112">Parent elements</span></span>

<span data-ttu-id="7d6bb-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7d6bb-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7d6bb-114">注釈</span><span class="sxs-lookup"><span data-stu-id="7d6bb-114">Remarks</span></span>

<span data-ttu-id="7d6bb-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7d6bb-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7d6bb-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7d6bb-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d6bb-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7d6bb-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d6bb-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="7d6bb-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7d6bb-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7d6bb-119">Schema Name</span></span>  <br/> |<span data-ttu-id="7d6bb-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7d6bb-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7d6bb-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7d6bb-121">Validation File</span></span>  <br/> |<span data-ttu-id="7d6bb-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7d6bb-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7d6bb-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7d6bb-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d6bb-124">正しい</span><span class="sxs-lookup"><span data-stu-id="7d6bb-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d6bb-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="7d6bb-125">See also</span></span>



- [<span data-ttu-id="7d6bb-126">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7d6bb-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

