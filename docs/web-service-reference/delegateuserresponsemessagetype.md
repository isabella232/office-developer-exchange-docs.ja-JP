---
title: DelegateUserResponseMessageType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUserResponseMessageType
api_type:
- schema
ms.assetid: 3dc9552c-1e2d-40ac-a137-827883c2bb88
description: DelegateUserResponseMessageType 要素には、1 つのデリゲートのユーザーの応答メッセージが含まれています。
ms.openlocfilehash: ac99e0ca219fc1f1e117f9288d895e27a1df4700
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759958"
---
# <a name="delegateuserresponsemessagetype"></a><span data-ttu-id="c1e70-103">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="c1e70-103">DelegateUserResponseMessageType</span></span>

<span data-ttu-id="c1e70-104">**DelegateUserResponseMessageType**要素には、1 つのデリゲートのユーザーの応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c1e70-104">The **DelegateUserResponseMessageType** element contains the response message for a single delegate user.</span></span> 
  
```xml
<DelegateUserResponseMessageType>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DelegateUser/>
</DelegateUserResponseMessageType>
```

<span data-ttu-id="c1e70-105">**DelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c1e70-105">**DelegateUserResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c1e70-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c1e70-106">Attributes and elements</span></span>

<span data-ttu-id="c1e70-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c1e70-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1e70-108">属性</span><span class="sxs-lookup"><span data-stu-id="c1e70-108">Attributes</span></span>

<span data-ttu-id="c1e70-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c1e70-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1e70-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c1e70-110">Child elements</span></span>

|<span data-ttu-id="c1e70-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="c1e70-111">**Element**</span></span>|<span data-ttu-id="c1e70-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c1e70-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1e70-113">MessageText</span><span class="sxs-lookup"><span data-stu-id="c1e70-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c1e70-114">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="c1e70-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c1e70-115">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c1e70-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c1e70-116">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="c1e70-116">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="c1e70-117">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c1e70-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c1e70-118">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="c1e70-118">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="c1e70-119">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c1e70-119">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="c1e70-120">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c1e70-120">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c1e70-121">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c1e70-121">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="c1e70-122">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="c1e70-122">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="c1e70-123">代理人の管理の応答で返される 1 つのデリゲートを識別します。</span><span class="sxs-lookup"><span data-stu-id="c1e70-123">Identifies a single delegate that is returned in a delegate management response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c1e70-124">親要素</span><span class="sxs-lookup"><span data-stu-id="c1e70-124">Parent elements</span></span>

|<span data-ttu-id="c1e70-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="c1e70-125">**Element**</span></span>|<span data-ttu-id="c1e70-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="c1e70-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1e70-127">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="c1e70-127">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="c1e70-128">Exchange Web サービス代理人の管理要求の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c1e70-128">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c1e70-129">備考</span><span class="sxs-lookup"><span data-stu-id="c1e70-129">Remarks</span></span>

<span data-ttu-id="c1e70-130">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c1e70-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1e70-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="c1e70-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1e70-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="c1e70-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c1e70-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c1e70-133">Schema Name</span></span>  <br/> |<span data-ttu-id="c1e70-134">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="c1e70-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c1e70-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c1e70-135">Validation File</span></span>  <br/> |<span data-ttu-id="c1e70-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c1e70-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c1e70-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c1e70-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="c1e70-138">False</span><span class="sxs-lookup"><span data-stu-id="c1e70-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1e70-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="c1e70-139">See also</span></span>

- [<span data-ttu-id="c1e70-140">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="c1e70-140">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="c1e70-141">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="c1e70-141">GetDelegate operation</span></span>](getdelegate-operation.md) 
- [<span data-ttu-id="c1e70-142">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="c1e70-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="c1e70-143">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="c1e70-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)
- [<span data-ttu-id="c1e70-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c1e70-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

