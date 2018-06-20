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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833193"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a><span data-ttu-id="dd384-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="dd384-103">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>

<span data-ttu-id="dd384-104">**ResponseMessages**要素には、Exchange Web サービスの代理人の管理要求の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="dd384-104">The **ResponseMessages** element contains the response messages for an Exchange Web Services delegate management request.</span></span> 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="dd384-105">**ArrayOfDelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="dd384-105">**ArrayOfDelegateUserResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd384-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dd384-106">Attributes and elements</span></span>

<span data-ttu-id="dd384-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dd384-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd384-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd384-108">Attributes</span></span>

<span data-ttu-id="dd384-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dd384-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd384-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dd384-110">Child elements</span></span>

|<span data-ttu-id="dd384-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="dd384-111">**Element**</span></span>|<span data-ttu-id="dd384-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dd384-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd384-113">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="dd384-113">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="dd384-114">代理人の管理操作の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="dd384-114">Contains response messages for delegate management operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dd384-115">親要素</span><span class="sxs-lookup"><span data-stu-id="dd384-115">Parent elements</span></span>

|<span data-ttu-id="dd384-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="dd384-116">**Element**</span></span>|<span data-ttu-id="dd384-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="dd384-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd384-118">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="dd384-118">AddDelegateResponse</span></span>](adddelegateresponse.md) <br/> |<span data-ttu-id="dd384-119">[AddDelegate 操作](adddelegate-operation.md)要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="dd384-119">Contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="dd384-120">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="dd384-120">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="dd384-121">状態と[GetDelegate の操作](getdelegate-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dd384-121">Contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="dd384-122">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="dd384-122">UpdateDelegateResponse</span></span>](updatedelegateresponse.md) <br/> |<span data-ttu-id="dd384-123">状態と[UpdateDelegate の操作](updatedelegate-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dd384-123">Contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="dd384-124">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="dd384-124">RemoveDelegateResponse</span></span>](removedelegateresponse.md) <br/> |<span data-ttu-id="dd384-125">状態と[RemoveDelegate の操作](removedelegate-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dd384-125">Contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dd384-126">備考</span><span class="sxs-lookup"><span data-stu-id="dd384-126">Remarks</span></span>

<span data-ttu-id="dd384-127">[AddDelegate 操作](adddelegate-operation.md)、 [GetDelegate 操作](getdelegate-operation.md)、 [UpdateDelegate の操作](updatedelegate-operation.md)、および[RemoveDelegate 操作](removedelegate-operation.md)では、この要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="dd384-127">This element is used in the [AddDelegate operation](adddelegate-operation.md), the [GetDelegate operation](getdelegate-operation.md), the [UpdateDelegate operation](updatedelegate-operation.md), and the [RemoveDelegate operation](removedelegate-operation.md).</span></span> <span data-ttu-id="dd384-128">代理人の管理操作の応答は、その他の応答とは異なる構成されています。</span><span class="sxs-lookup"><span data-stu-id="dd384-128">The delegate management operation responses are structured differently than other responses.</span></span> <span data-ttu-id="dd384-129">代理人の管理の応答メッセージは、厳密型指定されました。</span><span class="sxs-lookup"><span data-stu-id="dd384-129">The delegate management response messages are strongly typed.</span></span>
  
<span data-ttu-id="dd384-130">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="dd384-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd384-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="dd384-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd384-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="dd384-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dd384-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dd384-133">Schema Name</span></span>  <br/> |<span data-ttu-id="dd384-134">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="dd384-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dd384-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dd384-135">Validation File</span></span>  <br/> |<span data-ttu-id="dd384-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dd384-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dd384-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dd384-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd384-138">False</span><span class="sxs-lookup"><span data-stu-id="dd384-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd384-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="dd384-139">See also</span></span>



[<span data-ttu-id="dd384-140">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="dd384-140">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="dd384-141">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="dd384-141">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="dd384-142">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="dd384-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
  
[<span data-ttu-id="dd384-143">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="dd384-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="dd384-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dd384-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

