---
title: 含む adddelegateresponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegateResponse
api_type:
- schema
ms.assetid: d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429
description: 含む adddelegateresponse 要素には、AddDelegate 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 1c38563ab38facf89fd5eab119542374949244c2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466459"
---
# <a name="adddelegateresponse"></a><span data-ttu-id="9b3ec-103">含む adddelegateresponse</span><span class="sxs-lookup"><span data-stu-id="9b3ec-103">AddDelegateResponse</span></span>

<span data-ttu-id="9b3ec-104">**含む adddelegateresponse**要素には、 [adddelegate 操作](adddelegate-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9b3ec-104">The **AddDelegateResponse** element contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span> 
  
```xml
<AddDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</AddDelegateResponse>
```

 <span data-ttu-id="9b3ec-105">**AddDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9b3ec-105">**AddDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b3ec-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9b3ec-106">Attributes and elements</span></span>

<span data-ttu-id="9b3ec-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9b3ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b3ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b3ec-108">Attributes</span></span>

<span data-ttu-id="9b3ec-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9b3ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b3ec-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9b3ec-110">Child elements</span></span>

|<span data-ttu-id="9b3ec-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9b3ec-111">**Element**</span></span>|<span data-ttu-id="9b3ec-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9b3ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b3ec-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="9b3ec-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="9b3ec-114">Exchange Web サービスの委任管理要求に対する応答メッセージが保存されています。</span><span class="sxs-lookup"><span data-stu-id="9b3ec-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="9b3ec-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="9b3ec-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9b3ec-116">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="9b3ec-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9b3ec-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9b3ec-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9b3ec-118">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="9b3ec-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9b3ec-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9b3ec-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9b3ec-120">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="9b3ec-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="9b3ec-121">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9b3ec-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9b3ec-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9b3ec-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9b3ec-123">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="9b3ec-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b3ec-124">親要素</span><span class="sxs-lookup"><span data-stu-id="9b3ec-124">Parent elements</span></span>

<span data-ttu-id="9b3ec-125">なし。</span><span class="sxs-lookup"><span data-stu-id="9b3ec-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9b3ec-126">注釈</span><span class="sxs-lookup"><span data-stu-id="9b3ec-126">Remarks</span></span>

<span data-ttu-id="9b3ec-127">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="9b3ec-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b3ec-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9b3ec-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b3ec-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="9b3ec-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9b3ec-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9b3ec-130">Schema Name</span></span>  <br/> |<span data-ttu-id="9b3ec-131">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9b3ec-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9b3ec-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9b3ec-132">Validation File</span></span>  <br/> |<span data-ttu-id="9b3ec-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9b3ec-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9b3ec-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9b3ec-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b3ec-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="9b3ec-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b3ec-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="9b3ec-136">See also</span></span>

- [<span data-ttu-id="9b3ec-137">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="9b3ec-137">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="9b3ec-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9b3ec-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="9b3ec-139">代理人の追加</span><span class="sxs-lookup"><span data-stu-id="9b3ec-139">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

