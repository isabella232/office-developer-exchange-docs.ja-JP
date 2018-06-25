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
description: ResponseMessages 要素には、Exchange Web サービスの代理人の管理要求の応答メッセージが含まれています。
ms.openlocfilehash: e4b5567f3ded003e9648eb8ebebfadf8f1748d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833193"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a><span data-ttu-id="aecaf-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="aecaf-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>

<span data-ttu-id="aecaf-104">**ResponseMessages**要素には、Exchange Web サービスの代理人の管理要求の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="aecaf-104">The **ResponseMessages** element contains the response messages for an Exchange Web Services delegate management request.</span></span> 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="aecaf-105">**ArrayOfDelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="aecaf-105">**ArrayOfDelegateUserResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aecaf-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="aecaf-106">Attributes and elements</span></span>

<span data-ttu-id="aecaf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aecaf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aecaf-108">属性</span><span class="sxs-lookup"><span data-stu-id="aecaf-108">Attributes</span></span>

<span data-ttu-id="aecaf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="aecaf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aecaf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="aecaf-110">Child elements</span></span>

|<span data-ttu-id="aecaf-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="aecaf-111">**Element**</span></span>|<span data-ttu-id="aecaf-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="aecaf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aecaf-113">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="aecaf-113">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="aecaf-114">代理人の管理操作の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="aecaf-114">Contains response messages for delegate management operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aecaf-115">親要素</span><span class="sxs-lookup"><span data-stu-id="aecaf-115">Parent elements</span></span>

|<span data-ttu-id="aecaf-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="aecaf-116">**Element**</span></span>|<span data-ttu-id="aecaf-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="aecaf-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aecaf-118">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="aecaf-118">AddDelegateResponse</span></span>](adddelegateresponse.md) <br/> |<span data-ttu-id="aecaf-119">[AddDelegate 操作](adddelegate-operation.md)要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="aecaf-119">Contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="aecaf-120">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="aecaf-120">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="aecaf-121">状態と[GetDelegate の操作](getdelegate-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aecaf-121">Contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="aecaf-122">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="aecaf-122">UpdateDelegateResponse</span></span>](updatedelegateresponse.md) <br/> |<span data-ttu-id="aecaf-123">状態と[UpdateDelegate の操作](updatedelegate-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aecaf-123">Contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="aecaf-124">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="aecaf-124">RemoveDelegateResponse</span></span>](removedelegateresponse.md) <br/> |<span data-ttu-id="aecaf-125">状態と[RemoveDelegate の操作](removedelegate-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aecaf-125">Contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aecaf-126">備考</span><span class="sxs-lookup"><span data-stu-id="aecaf-126">Remarks</span></span>

<span data-ttu-id="aecaf-127">[AddDelegate 操作](adddelegate-operation.md)、 [GetDelegate 操作](getdelegate-operation.md)、 [UpdateDelegate の操作](updatedelegate-operation.md)、および[RemoveDelegate 操作](removedelegate-operation.md)では、この要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="aecaf-127">This element is used in the [AddDelegate operation](adddelegate-operation.md), the [GetDelegate operation](getdelegate-operation.md), the [UpdateDelegate operation](updatedelegate-operation.md), and the [RemoveDelegate operation](removedelegate-operation.md).</span></span> <span data-ttu-id="aecaf-128">代理人の管理操作の応答は、その他の応答とは異なる構成されています。</span><span class="sxs-lookup"><span data-stu-id="aecaf-128">The delegate management operation responses are structured differently than other responses.</span></span> <span data-ttu-id="aecaf-129">代理人の管理の応答メッセージは、厳密型指定されました。</span><span class="sxs-lookup"><span data-stu-id="aecaf-129">The delegate management response messages are strongly typed.</span></span>
  
<span data-ttu-id="aecaf-130">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="aecaf-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aecaf-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="aecaf-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aecaf-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="aecaf-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aecaf-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aecaf-133">Schema Name</span></span>  <br/> |<span data-ttu-id="aecaf-134">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="aecaf-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aecaf-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aecaf-135">Validation File</span></span>  <br/> |<span data-ttu-id="aecaf-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aecaf-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aecaf-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="aecaf-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="aecaf-138">False</span><span class="sxs-lookup"><span data-stu-id="aecaf-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aecaf-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="aecaf-139">See also</span></span>



[<span data-ttu-id="aecaf-140">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="aecaf-140">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="aecaf-141">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="aecaf-141">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="aecaf-142">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="aecaf-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
  
[<span data-ttu-id="aecaf-143">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="aecaf-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="aecaf-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="aecaf-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

