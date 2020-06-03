---
title: ResponseMessages (ArrayOfDelegateUserResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 14819975-ce54-4f0e-9f90-d4b275895ea0
description: ResponseMessages 要素には、Exchange Web サービスの委任管理要求に対する応答メッセージが含まれています。
ms.openlocfilehash: 6b035f4ee46af1750a275e2c61b2cddea06b37a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465458"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a><span data-ttu-id="3ad10-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="3ad10-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>

<span data-ttu-id="3ad10-104">**Responsemessages**要素には、Exchange Web サービスの委任管理要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3ad10-104">The **ResponseMessages** element contains the response messages for an Exchange Web Services delegate management request.</span></span> 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="3ad10-105">**ArrayOfDelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3ad10-105">**ArrayOfDelegateUserResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3ad10-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3ad10-106">Attributes and elements</span></span>

<span data-ttu-id="3ad10-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3ad10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3ad10-108">属性</span><span class="sxs-lookup"><span data-stu-id="3ad10-108">Attributes</span></span>

<span data-ttu-id="3ad10-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3ad10-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3ad10-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3ad10-110">Child elements</span></span>

|<span data-ttu-id="3ad10-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="3ad10-111">**Element**</span></span>|<span data-ttu-id="3ad10-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3ad10-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3ad10-113">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="3ad10-113">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="3ad10-114">代理人管理操作の応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="3ad10-114">Contains response messages for delegate management operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3ad10-115">親要素</span><span class="sxs-lookup"><span data-stu-id="3ad10-115">Parent elements</span></span>

|<span data-ttu-id="3ad10-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="3ad10-116">**Element**</span></span>|<span data-ttu-id="3ad10-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="3ad10-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3ad10-118">含む adddelegateresponse</span><span class="sxs-lookup"><span data-stu-id="3ad10-118">AddDelegateResponse</span></span>](adddelegateresponse.md) <br/> |<span data-ttu-id="3ad10-119">[Adddelegate 操作](adddelegate-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="3ad10-119">Contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="3ad10-120">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="3ad10-120">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="3ad10-121">[Getdelegate 操作](getdelegate-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="3ad10-121">Contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="3ad10-122">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="3ad10-122">UpdateDelegateResponse</span></span>](updatedelegateresponse.md) <br/> |<span data-ttu-id="3ad10-123">[代理人操作](updatedelegate-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="3ad10-123">Contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="3ad10-124">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="3ad10-124">RemoveDelegateResponse</span></span>](removedelegateresponse.md) <br/> |<span data-ttu-id="3ad10-125">[Removedelegate 操作](removedelegate-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="3ad10-125">Contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3ad10-126">注釈</span><span class="sxs-lookup"><span data-stu-id="3ad10-126">Remarks</span></span>

<span data-ttu-id="3ad10-127">この要素は、 [Adddelegate 操作](adddelegate-operation.md)、 [Getdelegate](getdelegate-operation.md)操作、 [Updatedelegate 操作](updatedelegate-operation.md)、および[removedelegate 操作](removedelegate-operation.md)で使用されます。</span><span class="sxs-lookup"><span data-stu-id="3ad10-127">This element is used in the [AddDelegate operation](adddelegate-operation.md), the [GetDelegate operation](getdelegate-operation.md), the [UpdateDelegate operation](updatedelegate-operation.md), and the [RemoveDelegate operation](removedelegate-operation.md).</span></span> <span data-ttu-id="3ad10-128">代理人管理操作の応答は、他の応答とは異なる構造になっています。</span><span class="sxs-lookup"><span data-stu-id="3ad10-128">The delegate management operation responses are structured differently than other responses.</span></span> <span data-ttu-id="3ad10-129">代理人管理応答メッセージは厳密に型指定されます。</span><span class="sxs-lookup"><span data-stu-id="3ad10-129">The delegate management response messages are strongly typed.</span></span>
  
<span data-ttu-id="3ad10-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3ad10-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3ad10-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3ad10-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3ad10-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="3ad10-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3ad10-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3ad10-133">Schema Name</span></span>  <br/> |<span data-ttu-id="3ad10-134">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3ad10-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3ad10-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3ad10-135">Validation File</span></span>  <br/> |<span data-ttu-id="3ad10-136">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3ad10-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3ad10-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3ad10-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="3ad10-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="3ad10-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3ad10-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="3ad10-139">See also</span></span>



[<span data-ttu-id="3ad10-140">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="3ad10-140">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="3ad10-141">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="3ad10-141">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="3ad10-142">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="3ad10-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
  
[<span data-ttu-id="3ad10-143">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="3ad10-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="3ad10-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3ad10-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

