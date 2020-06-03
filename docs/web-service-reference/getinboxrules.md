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
description: Getinbox Rules 要素は、サーバーストア内のメールボックスの受信トレイルールを取得する要求を定義します。
ms.openlocfilehash: 890592fd3f87fc5592a618a2febf28e4daf0dbe4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457929"
---
# <a name="getinboxrules"></a><span data-ttu-id="af0ce-103">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="af0ce-103">GetInboxRules</span></span>

<span data-ttu-id="af0ce-104">**Getinbox rules**要素は、サーバーストア内のメールボックスの受信トレイルールを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="af0ce-104">The **GetInboxRules** element defines a request to get the Inbox rules on a mailbox in the server store.</span></span> 
  
```XML
<GetInboxRules>
   <MailboxSmtpAddress/>
</GetInboxRules>
```

 <span data-ttu-id="af0ce-105">**Get受信規則 Requesttype**</span><span class="sxs-lookup"><span data-stu-id="af0ce-105">**GetInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af0ce-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="af0ce-106">Attributes and elements</span></span>

<span data-ttu-id="af0ce-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="af0ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af0ce-108">属性</span><span class="sxs-lookup"><span data-stu-id="af0ce-108">Attributes</span></span>

<span data-ttu-id="af0ce-109">なし。</span><span class="sxs-lookup"><span data-stu-id="af0ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af0ce-110">子要素</span><span class="sxs-lookup"><span data-stu-id="af0ce-110">Child elements</span></span>

|<span data-ttu-id="af0ce-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="af0ce-111">**Element**</span></span>|<span data-ttu-id="af0ce-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="af0ce-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af0ce-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="af0ce-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="af0ce-114">受信トレイルールを取得するユーザーの SMTP アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="af0ce-114">Represents the SMTP address of the user whose Inbox rules are to be retrieved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="af0ce-115">親要素</span><span class="sxs-lookup"><span data-stu-id="af0ce-115">Parent elements</span></span>

<span data-ttu-id="af0ce-116">なし。</span><span class="sxs-lookup"><span data-stu-id="af0ce-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="af0ce-117">注釈</span><span class="sxs-lookup"><span data-stu-id="af0ce-117">Remarks</span></span>

<span data-ttu-id="af0ce-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="af0ce-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af0ce-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="af0ce-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af0ce-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="af0ce-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="af0ce-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="af0ce-121">Schema Name</span></span>  <br/> |<span data-ttu-id="af0ce-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="af0ce-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="af0ce-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="af0ce-123">Validation File</span></span>  <br/> |<span data-ttu-id="af0ce-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="af0ce-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="af0ce-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="af0ce-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="af0ce-126">正しい</span><span class="sxs-lookup"><span data-stu-id="af0ce-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af0ce-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="af0ce-127">See also</span></span>



[<span data-ttu-id="af0ce-128">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="af0ce-128">GetInboxRules operation</span></span>](getinboxrules-operation.md)

