---
title: GetInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRules
api_type:
- schema
ms.assetid: 7a54992d-03a6-4afc-a2e4-dcdc9ce54194
description: GetInboxRules 要素は、サーバー ストア内のメールボックスの受信トレイ ルールを取得する要求を定義します。
ms.openlocfilehash: 3c3ee682dd009e5c4bec940637a7dfa3c11f8402
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760760"
---
# <a name="getinboxrules"></a><span data-ttu-id="cf7c9-103">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="cf7c9-103">GetInboxRules</span></span>

<span data-ttu-id="cf7c9-104">**GetInboxRules**要素は、サーバー ストア内のメールボックスの受信トレイ ルールを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="cf7c9-104">The **GetInboxRules** element defines a request to get the Inbox rules on a mailbox in the server store.</span></span> 
  
```XML
<GetInboxRules>
   <MailboxSmtpAddress/>
</GetInboxRules>
```

 <span data-ttu-id="cf7c9-105">**GetInboxRulesRequestType**</span><span class="sxs-lookup"><span data-stu-id="cf7c9-105">**GetInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf7c9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cf7c9-106">Attributes and elements</span></span>

<span data-ttu-id="cf7c9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cf7c9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf7c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="cf7c9-108">Attributes</span></span>

<span data-ttu-id="cf7c9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cf7c9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf7c9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cf7c9-110">Child elements</span></span>

|<span data-ttu-id="cf7c9-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="cf7c9-111">**Element**</span></span>|<span data-ttu-id="cf7c9-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="cf7c9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf7c9-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="cf7c9-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="cf7c9-114">受信トレイ ルールを取得するのには、ユーザーの SMTP アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="cf7c9-114">Represents the SMTP address of the user whose Inbox rules are to be retrieved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf7c9-115">親要素</span><span class="sxs-lookup"><span data-stu-id="cf7c9-115">Parent elements</span></span>

<span data-ttu-id="cf7c9-116">なし。</span><span class="sxs-lookup"><span data-stu-id="cf7c9-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cf7c9-117">備考</span><span class="sxs-lookup"><span data-stu-id="cf7c9-117">Remarks</span></span>

<span data-ttu-id="cf7c9-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cf7c9-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf7c9-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="cf7c9-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf7c9-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="cf7c9-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cf7c9-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cf7c9-121">Schema Name</span></span>  <br/> |<span data-ttu-id="cf7c9-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="cf7c9-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cf7c9-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cf7c9-123">Validation File</span></span>  <br/> |<span data-ttu-id="cf7c9-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cf7c9-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cf7c9-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cf7c9-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf7c9-126">True</span><span class="sxs-lookup"><span data-stu-id="cf7c9-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf7c9-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="cf7c9-127">See also</span></span>



[<span data-ttu-id="cf7c9-128">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="cf7c9-128">GetInboxRules operation</span></span>](getinboxrules-operation.md)

