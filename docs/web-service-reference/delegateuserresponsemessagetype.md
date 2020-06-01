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
description: DelegateUserResponseMessageType 要素には、1人の代理ユーザーに対する応答メッセージが含まれています。
ms.openlocfilehash: d7addac2ef05d50e0043490ac20d299ece7d577b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457383"
---
# <a name="delegateuserresponsemessagetype"></a><span data-ttu-id="7e55b-103">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="7e55b-103">DelegateUserResponseMessageType</span></span>

<span data-ttu-id="7e55b-104">**DelegateUserResponseMessageType**要素には、1人の代理ユーザーに対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e55b-104">The **DelegateUserResponseMessageType** element contains the response message for a single delegate user.</span></span> 
  
```xml
<DelegateUserResponseMessageType>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DelegateUser/>
</DelegateUserResponseMessageType>
```

<span data-ttu-id="7e55b-105">**DelegateUserResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="7e55b-105">**DelegateUserResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7e55b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7e55b-106">Attributes and elements</span></span>

<span data-ttu-id="7e55b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e55b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e55b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e55b-108">Attributes</span></span>

<span data-ttu-id="7e55b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7e55b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e55b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7e55b-110">Child elements</span></span>

|<span data-ttu-id="7e55b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7e55b-111">**Element**</span></span>|<span data-ttu-id="7e55b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e55b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e55b-113">MessageText</span><span class="sxs-lookup"><span data-stu-id="7e55b-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7e55b-114">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="7e55b-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7e55b-115">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7e55b-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7e55b-116">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="7e55b-116">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="7e55b-117">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7e55b-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7e55b-118">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="7e55b-118">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="7e55b-119">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e55b-119">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7e55b-120">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7e55b-120">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7e55b-121">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="7e55b-121">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7e55b-122">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="7e55b-122">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="7e55b-123">代理人管理応答で返される1つの代理人を識別します。</span><span class="sxs-lookup"><span data-stu-id="7e55b-123">Identifies a single delegate that is returned in a delegate management response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e55b-124">親要素</span><span class="sxs-lookup"><span data-stu-id="7e55b-124">Parent elements</span></span>

|<span data-ttu-id="7e55b-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e55b-125">**Element**</span></span>|<span data-ttu-id="7e55b-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e55b-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e55b-127">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="7e55b-127">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="7e55b-128">Exchange Web サービスの委任管理要求に対する応答メッセージが保存されています。</span><span class="sxs-lookup"><span data-stu-id="7e55b-128">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e55b-129">注釈</span><span class="sxs-lookup"><span data-stu-id="7e55b-129">Remarks</span></span>

<span data-ttu-id="7e55b-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7e55b-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e55b-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7e55b-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e55b-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e55b-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e55b-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e55b-133">Schema Name</span></span>  <br/> |<span data-ttu-id="7e55b-134">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7e55b-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7e55b-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e55b-135">Validation File</span></span>  <br/> |<span data-ttu-id="7e55b-136">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7e55b-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e55b-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7e55b-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e55b-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="7e55b-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e55b-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e55b-139">See also</span></span>

- [<span data-ttu-id="7e55b-140">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="7e55b-140">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="7e55b-141">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="7e55b-141">GetDelegate operation</span></span>](getdelegate-operation.md) 
- [<span data-ttu-id="7e55b-142">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="7e55b-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="7e55b-143">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="7e55b-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)
- [<span data-ttu-id="7e55b-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7e55b-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

