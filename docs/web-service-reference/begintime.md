---
title: BeginTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2a60c89c-9c21-4041-9593-b244ac1608ef
description: BeginTime 要素は、事前通知に対してクエリを実行する時間間隔の開始を指定します。
ms.openlocfilehash: 4f926b8e4931c187cd4d5b97d6182d609bc15a1b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463378"
---
# <a name="begintime"></a><span data-ttu-id="19ded-103">BeginTime</span><span class="sxs-lookup"><span data-stu-id="19ded-103">BeginTime</span></span>

<span data-ttu-id="19ded-104">**Begintime**要素は、事前通知に対してクエリを実行する時間間隔の開始を指定します。</span><span class="sxs-lookup"><span data-stu-id="19ded-104">The **BeginTime** element specifies the beginning of the time span to query for reminders.</span></span> 
  
```XML
<BeginTime/>
```

 <span data-ttu-id="19ded-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="19ded-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19ded-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="19ded-106">Attributes and elements</span></span>

<span data-ttu-id="19ded-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="19ded-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19ded-108">属性</span><span class="sxs-lookup"><span data-stu-id="19ded-108">Attributes</span></span>

<span data-ttu-id="19ded-109">なし。</span><span class="sxs-lookup"><span data-stu-id="19ded-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19ded-110">子要素</span><span class="sxs-lookup"><span data-stu-id="19ded-110">Child elements</span></span>

<span data-ttu-id="19ded-111">なし。</span><span class="sxs-lookup"><span data-stu-id="19ded-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19ded-112">親要素</span><span class="sxs-lookup"><span data-stu-id="19ded-112">Parent elements</span></span>

[<span data-ttu-id="19ded-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="19ded-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="19ded-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="19ded-114">Text value</span></span>

<span data-ttu-id="19ded-115">**Begintime**要素のテキスト値は、アラームがあるアイテムの開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="19ded-115">The text value of the **BeginTime** element is the beginning time of the item the reminder is for.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="19ded-116">注釈</span><span class="sxs-lookup"><span data-stu-id="19ded-116">Remarks</span></span>

<span data-ttu-id="19ded-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="19ded-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="19ded-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="19ded-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19ded-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="19ded-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19ded-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="19ded-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="19ded-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="19ded-121">Schema Name</span></span>  <br/> |<span data-ttu-id="19ded-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="19ded-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="19ded-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="19ded-123">Validation File</span></span>  <br/> |<span data-ttu-id="19ded-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="19ded-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="19ded-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="19ded-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="19ded-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="19ded-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19ded-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="19ded-127">See also</span></span>



[<span data-ttu-id="19ded-128">GetReminders</span><span class="sxs-lookup"><span data-stu-id="19ded-128">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="19ded-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="19ded-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

