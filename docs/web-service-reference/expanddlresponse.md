---
title: ExpandDLResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDLResponse
api_type:
- schema
ms.assetid: 1c60dd64-a083-460a-9840-021d30f871d6
description: ExpandDLResponse 要素は、配布リストを展開する要求への応答を定義します。
ms.openlocfilehash: a5b162fe2c29f760b7499e9e946b700ce69be970
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456942"
---
# <a name="expanddlresponse"></a><span data-ttu-id="b702f-103">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="b702f-103">ExpandDLResponse</span></span>

<span data-ttu-id="b702f-104">**Expanddlresponse**要素は、配布リストを展開する要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="b702f-104">The **ExpandDLResponse** element defines a response to a request to expand a distribution list.</span></span> 
  
[<span data-ttu-id="b702f-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="b702f-105">ExpandDLResponse</span></span>](expanddlresponse.md)
  
```xml
<ExpandDLResponse>
   <ResponseMessages/>
</ExpandDLResponse>
```

 <span data-ttu-id="b702f-106">**ExpandDLResponseType**</span><span class="sxs-lookup"><span data-stu-id="b702f-106">**ExpandDLResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b702f-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b702f-107">Attributes and elements</span></span>

<span data-ttu-id="b702f-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b702f-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b702f-109">属性</span><span class="sxs-lookup"><span data-stu-id="b702f-109">Attributes</span></span>

<span data-ttu-id="b702f-110">なし。</span><span class="sxs-lookup"><span data-stu-id="b702f-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b702f-111">子要素</span><span class="sxs-lookup"><span data-stu-id="b702f-111">Child elements</span></span>

|<span data-ttu-id="b702f-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="b702f-112">**Element**</span></span>|<span data-ttu-id="b702f-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="b702f-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b702f-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b702f-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b702f-115">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="b702f-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b702f-116">親要素</span><span class="sxs-lookup"><span data-stu-id="b702f-116">Parent elements</span></span>

<span data-ttu-id="b702f-117">なし。</span><span class="sxs-lookup"><span data-stu-id="b702f-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b702f-118">注釈</span><span class="sxs-lookup"><span data-stu-id="b702f-118">Remarks</span></span>

<span data-ttu-id="b702f-119">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b702f-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b702f-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b702f-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b702f-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="b702f-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b702f-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b702f-122">Schema name</span></span>  <br/> |<span data-ttu-id="b702f-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b702f-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="b702f-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b702f-124">Validation file</span></span>  <br/> |<span data-ttu-id="b702f-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b702f-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b702f-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b702f-126">Can be empty</span></span>  <br/> |<span data-ttu-id="b702f-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="b702f-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b702f-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="b702f-128">See also</span></span>



[<span data-ttu-id="b702f-129">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="b702f-129">ExpandDL</span></span>](expanddl.md)
  
[<span data-ttu-id="b702f-130">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="b702f-130">ExpandDL operation</span></span>](expanddl-operation.md)

