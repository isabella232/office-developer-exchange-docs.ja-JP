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
description: UpdateInboxRules 要素は、サーバー ストア内のメールボックスの受信トレイ ルールを更新する要求を定義します。
ms.openlocfilehash: 73af3efcbf4320604576b724acf18530b8b86b26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839854"
---
# <a name="updateinboxrules"></a><span data-ttu-id="3285c-103">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="3285c-103">UpdateInboxRules</span></span>

<span data-ttu-id="3285c-104">**UpdateInboxRules**要素は、サーバー ストア内のメールボックスの受信トレイ ルールを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="3285c-104">The **UpdateInboxRules** element defines a request to update the Inbox rules in a mailbox in the server store.</span></span> 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 <span data-ttu-id="3285c-105">**UpdateInboxRulesRequestType**</span><span class="sxs-lookup"><span data-stu-id="3285c-105">**UpdateInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3285c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3285c-106">Attributes and elements</span></span>

<span data-ttu-id="3285c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3285c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3285c-108">属性</span><span class="sxs-lookup"><span data-stu-id="3285c-108">Attributes</span></span>

<span data-ttu-id="3285c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3285c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3285c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3285c-110">Child elements</span></span>

|<span data-ttu-id="3285c-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3285c-111">**Element**</span></span>|<span data-ttu-id="3285c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3285c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3285c-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="3285c-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="3285c-114">受信トレイ ルールを作成、変更、または削除するのにはユーザーの SMTP アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="3285c-114">Represents the SMTP address of the user whose Inbox rules are to be created, modified, or deleted.</span></span>  <br/> |
|[<span data-ttu-id="3285c-115">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="3285c-115">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md) <br/> |<span data-ttu-id="3285c-116">Microsoft Outlook のルールの blob を削除するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3285c-116">Indicates whether to remove the Microsoft Outlook rule blob.</span></span>  <br/> |
|[<span data-ttu-id="3285c-117">Operations</span><span class="sxs-lookup"><span data-stu-id="3285c-117">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="3285c-118">受信トレイ ルール操作の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3285c-118">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3285c-119">親要素</span><span class="sxs-lookup"><span data-stu-id="3285c-119">Parent elements</span></span>

<span data-ttu-id="3285c-120">なし。</span><span class="sxs-lookup"><span data-stu-id="3285c-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3285c-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3285c-121">Text value</span></span>

<span data-ttu-id="3285c-122">なし。</span><span class="sxs-lookup"><span data-stu-id="3285c-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3285c-123">備考</span><span class="sxs-lookup"><span data-stu-id="3285c-123">Remarks</span></span>

<span data-ttu-id="3285c-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3285c-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3285c-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="3285c-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3285c-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="3285c-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3285c-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3285c-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3285c-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="3285c-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3285c-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3285c-129">Validation File</span></span>  <br/> |<span data-ttu-id="3285c-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3285c-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3285c-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3285c-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="3285c-132">True</span><span class="sxs-lookup"><span data-stu-id="3285c-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3285c-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="3285c-133">See also</span></span>



[<span data-ttu-id="3285c-134">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="3285c-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="3285c-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3285c-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

