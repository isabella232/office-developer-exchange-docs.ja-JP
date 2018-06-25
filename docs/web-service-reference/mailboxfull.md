---
title: MailboxFull
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxFull
api_type:
- schema
ms.assetid: 38b28c9b-9da2-4d6a-9cda-9c393986575b
description: MailboxFull 要素は、受信者のメールボックスがいっぱいであるかどうかを示します。
ms.openlocfilehash: 8e2c9e01b93af03e875834724a942cd9b17a73f3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832286"
---
# <a name="mailboxfull"></a><span data-ttu-id="b0433-103">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="b0433-103">MailboxFull</span></span>

<span data-ttu-id="b0433-104">**MailboxFull**要素は、受信者のメールボックスがいっぱいであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b0433-104">The **MailboxFull** element indicates whether the mailbox for the recipient is full.</span></span> 
  
```XML
<MailboxFull>true | false</MailboxFull>
```

<span data-ttu-id="b0433-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="b0433-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b0433-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b0433-106">Attributes and elements</span></span>

<span data-ttu-id="b0433-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b0433-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0433-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0433-108">Attributes</span></span>

<span data-ttu-id="b0433-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b0433-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0433-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b0433-110">Child elements</span></span>

<span data-ttu-id="b0433-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b0433-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b0433-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b0433-112">Parent elements</span></span>

|<span data-ttu-id="b0433-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b0433-113">**Element**</span></span>|<span data-ttu-id="b0433-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0433-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0433-115">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="b0433-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="b0433-116">さまざまな種類のメール ヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="b0433-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b0433-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b0433-117">Text value</span></span>

<span data-ttu-id="b0433-118">この要素には、 **true**または**false**のいずれかができます。</span><span class="sxs-lookup"><span data-stu-id="b0433-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="b0433-119">**True**の場合は、メールボックスの容量に達したことを示します**false**の場合、それに達していない容量を示します。</span><span class="sxs-lookup"><span data-stu-id="b0433-119">A value of **true** indicates that the mailbox has reached its capacity; a value of **false** indicates that it has not reached capacity.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b0433-120">備考</span><span class="sxs-lookup"><span data-stu-id="b0433-120">Remarks</span></span>

<span data-ttu-id="b0433-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b0433-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0433-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="b0433-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0433-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="b0433-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0433-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b0433-124">Schema Name</span></span>  <br/> |<span data-ttu-id="b0433-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b0433-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0433-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b0433-126">Validation File</span></span>  <br/> |<span data-ttu-id="b0433-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b0433-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0433-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b0433-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0433-129">False</span><span class="sxs-lookup"><span data-stu-id="b0433-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0433-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0433-130">See also</span></span>

- [<span data-ttu-id="b0433-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b0433-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

