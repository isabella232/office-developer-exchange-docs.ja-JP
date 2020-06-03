---
title: DeleteFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderResponse
api_type:
- schema
ms.assetid: 27578bda-ef0a-4a33-bccc-2c1bc1735424
description: DeleteFolderResponse 要素は、DeleteFolder 要求への応答を定義します。
ms.openlocfilehash: 58b814662c769784c5fd682a9e039863a9787d8d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458489"
---
# <a name="deletefolderresponse"></a><span data-ttu-id="8ff97-103">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="8ff97-103">DeleteFolderResponse</span></span>

<span data-ttu-id="8ff97-104">**Deletefolderresponse**要素は、deletefolder 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="8ff97-104">The **DeleteFolderResponse** element defines a response to a DeleteFolder request.</span></span> 
  
```xml
<DeleteFolderResponse>
   <ResponseMessages/>
</DeleteFolderResponse>
```

 <span data-ttu-id="8ff97-105">**DeleteFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="8ff97-105">**DeleteFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ff97-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8ff97-106">Attributes and elements</span></span>

<span data-ttu-id="8ff97-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8ff97-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ff97-108">属性</span><span class="sxs-lookup"><span data-stu-id="8ff97-108">Attributes</span></span>

<span data-ttu-id="8ff97-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8ff97-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ff97-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8ff97-110">Child elements</span></span>

|<span data-ttu-id="8ff97-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="8ff97-111">**Element**</span></span>|<span data-ttu-id="8ff97-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8ff97-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ff97-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8ff97-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="8ff97-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="8ff97-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8ff97-115">親要素</span><span class="sxs-lookup"><span data-stu-id="8ff97-115">Parent elements</span></span>

<span data-ttu-id="8ff97-116">なし。</span><span class="sxs-lookup"><span data-stu-id="8ff97-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8ff97-117">注釈</span><span class="sxs-lookup"><span data-stu-id="8ff97-117">Remarks</span></span>

<span data-ttu-id="8ff97-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8ff97-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ff97-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8ff97-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ff97-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="8ff97-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8ff97-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8ff97-121">Schema name</span></span>  <br/> |<span data-ttu-id="8ff97-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="8ff97-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8ff97-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8ff97-123">Validation file</span></span>  <br/> |<span data-ttu-id="8ff97-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="8ff97-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8ff97-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8ff97-125">Can be empty</span></span>  <br/> |<span data-ttu-id="8ff97-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="8ff97-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ff97-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="8ff97-127">See also</span></span>

- [<span data-ttu-id="8ff97-128">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="8ff97-128">DeleteFolder operation</span></span>](deletefolder-operation.md) 
- [<span data-ttu-id="8ff97-129">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="8ff97-129">DeleteFolder</span></span>](deletefolder.md)
- [<span data-ttu-id="8ff97-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8ff97-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

