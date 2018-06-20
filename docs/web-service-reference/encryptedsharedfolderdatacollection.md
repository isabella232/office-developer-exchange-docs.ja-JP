---
title: EncryptedSharedFolderDataCollection
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EncryptedSharedFolderDataCollection
api_type:
- schema
ms.assetid: 25c6ae87-bbb9-4dd5-a85a-d669fcea137f
description: EncryptedSharedFolderDataCollection 要素には、クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントとデータ構造体のコレクションが含まれています。
ms.openlocfilehash: e4d37f5df10f5e270be5126479485239f2205d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760273"
---
# <a name="encryptedsharedfolderdatacollection"></a><span data-ttu-id="3276a-103">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="3276a-103">EncryptedSharedFolderDataCollection</span></span>

<span data-ttu-id="3276a-104">**EncryptedSharedFolderDataCollection**要素には、クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントとデータ構造体のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3276a-104">The **EncryptedSharedFolderDataCollection** element contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderDataCollection>   <EncryptedSharedFolderData/></EncryptedSharedFolderDataCollection>
```

 <span data-ttu-id="3276a-105">**ArrayOfEncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="3276a-105">**ArrayOfEncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3276a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3276a-106">Attributes and elements</span></span>

<span data-ttu-id="3276a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3276a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3276a-108">属性</span><span class="sxs-lookup"><span data-stu-id="3276a-108">Attributes</span></span>

<span data-ttu-id="3276a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3276a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3276a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3276a-110">Child elements</span></span>

|<span data-ttu-id="3276a-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3276a-111">**Element**</span></span>|<span data-ttu-id="3276a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3276a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3276a-113">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="3276a-113">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="3276a-114">クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントで暗号化されたデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3276a-114">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3276a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="3276a-115">Parent elements</span></span>

|<span data-ttu-id="3276a-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="3276a-116">**Element**</span></span>|<span data-ttu-id="3276a-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="3276a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3276a-118">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="3276a-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="3276a-119">[GetSharingMetadata 操作](getsharingmetadata-operation.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="3276a-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="3276a-120">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3276a-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="3276a-121">状態および 1 つの結果が含まれています[GetSharingMetadata の操作](getsharingmetadata-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="3276a-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3276a-122">備考</span><span class="sxs-lookup"><span data-stu-id="3276a-122">Remarks</span></span>

<span data-ttu-id="3276a-123">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3276a-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3276a-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="3276a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3276a-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="3276a-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3276a-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3276a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3276a-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="3276a-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3276a-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3276a-128">Validation File</span></span>  <br/> |<span data-ttu-id="3276a-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3276a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3276a-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3276a-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3276a-131">False</span><span class="sxs-lookup"><span data-stu-id="3276a-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3276a-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="3276a-132">See also</span></span>

- [<span data-ttu-id="3276a-133">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="3276a-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="3276a-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3276a-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

