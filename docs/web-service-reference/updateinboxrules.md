---
title: UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: d220064f-ff4d-4537-8077-adf94f2cbdbd
description: Updateinbox Rules 要素は、サーバーストア内のメールボックスの受信トレイルールを更新する要求を定義します。
ms.openlocfilehash: d604604d582d28c07eaa75d3239082d1b6735e65
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456361"
---
# <a name="updateinboxrules"></a><span data-ttu-id="94dab-103">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="94dab-103">UpdateInboxRules</span></span>

<span data-ttu-id="94dab-104">**Updateinbox rules**要素は、サーバーストア内のメールボックスの受信トレイルールを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="94dab-104">The **UpdateInboxRules** element defines a request to update the Inbox rules in a mailbox in the server store.</span></span> 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 <span data-ttu-id="94dab-105">**Update受信トレイルール Requesttype**</span><span class="sxs-lookup"><span data-stu-id="94dab-105">**UpdateInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94dab-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="94dab-106">Attributes and elements</span></span>

<span data-ttu-id="94dab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="94dab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94dab-108">属性</span><span class="sxs-lookup"><span data-stu-id="94dab-108">Attributes</span></span>

<span data-ttu-id="94dab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="94dab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94dab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="94dab-110">Child elements</span></span>

|<span data-ttu-id="94dab-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="94dab-111">**Element**</span></span>|<span data-ttu-id="94dab-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="94dab-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94dab-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="94dab-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="94dab-114">受信トレイルールを作成、変更、または削除するユーザーの SMTP アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="94dab-114">Represents the SMTP address of the user whose Inbox rules are to be created, modified, or deleted.</span></span>  <br/> |
|[<span data-ttu-id="94dab-115">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="94dab-115">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md) <br/> |<span data-ttu-id="94dab-116">Microsoft Outlook のルール blob を削除するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="94dab-116">Indicates whether to remove the Microsoft Outlook rule blob.</span></span>  <br/> |
|[<span data-ttu-id="94dab-117">Operations</span><span class="sxs-lookup"><span data-stu-id="94dab-117">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="94dab-118">受信トレイに対して実行できるルール操作の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="94dab-118">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="94dab-119">親要素</span><span class="sxs-lookup"><span data-stu-id="94dab-119">Parent elements</span></span>

<span data-ttu-id="94dab-120">なし。</span><span class="sxs-lookup"><span data-stu-id="94dab-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="94dab-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="94dab-121">Text value</span></span>

<span data-ttu-id="94dab-122">なし。</span><span class="sxs-lookup"><span data-stu-id="94dab-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="94dab-123">注釈</span><span class="sxs-lookup"><span data-stu-id="94dab-123">Remarks</span></span>

<span data-ttu-id="94dab-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="94dab-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94dab-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="94dab-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94dab-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="94dab-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="94dab-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="94dab-127">Schema Name</span></span>  <br/> |<span data-ttu-id="94dab-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="94dab-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="94dab-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="94dab-129">Validation File</span></span>  <br/> |<span data-ttu-id="94dab-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="94dab-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="94dab-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="94dab-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="94dab-132">正しい</span><span class="sxs-lookup"><span data-stu-id="94dab-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94dab-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="94dab-133">See also</span></span>



[<span data-ttu-id="94dab-134">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="94dab-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="94dab-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="94dab-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

