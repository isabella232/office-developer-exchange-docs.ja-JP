---
title: EncryptedSharedFolderData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EncryptedSharedFolderData
api_type:
- schema
ms.assetid: c1d4ca18-c5ce-41ff-bab4-f75e358c8b9f
description: EncryptedSharedFolderData 要素には、クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントで暗号化されたデータが含まれています。
ms.openlocfilehash: 63966e95becaab4b3b1e54aa81f1b20a8b09dfd3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760275"
---
# <a name="encryptedsharedfolderdata"></a><span data-ttu-id="63c47-103">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="63c47-103">EncryptedSharedFolderData</span></span>

<span data-ttu-id="63c47-104">**EncryptedSharedFolderData**要素には、クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントで暗号化されたデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="63c47-104">The **EncryptedSharedFolderData** element contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 <span data-ttu-id="63c47-105">**EncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="63c47-105">**EncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63c47-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="63c47-106">Attributes and elements</span></span>

<span data-ttu-id="63c47-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="63c47-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63c47-108">属性</span><span class="sxs-lookup"><span data-stu-id="63c47-108">Attributes</span></span>

<span data-ttu-id="63c47-109">なし。</span><span class="sxs-lookup"><span data-stu-id="63c47-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63c47-110">子要素</span><span class="sxs-lookup"><span data-stu-id="63c47-110">Child elements</span></span>

|<span data-ttu-id="63c47-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="63c47-111">**Element**</span></span>|<span data-ttu-id="63c47-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="63c47-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63c47-113">トークン</span><span class="sxs-lookup"><span data-stu-id="63c47-113">Token</span></span>](token.md) <br/> |<span data-ttu-id="63c47-114">共有データの識別トークンを表す暗号化されたデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="63c47-114">Contains encrypted data that represents the identification token for the shared data.</span></span>  <br/> |
|[<span data-ttu-id="63c47-115">Data</span><span class="sxs-lookup"><span data-stu-id="63c47-115">Data</span></span>](data.md) <br/> |<span data-ttu-id="63c47-116">共有データを表す暗号化されたデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="63c47-116">Contains encrypted data that represents the shared data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63c47-117">親要素</span><span class="sxs-lookup"><span data-stu-id="63c47-117">Parent elements</span></span>

|<span data-ttu-id="63c47-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="63c47-118">**Element**</span></span>|<span data-ttu-id="63c47-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="63c47-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63c47-120">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="63c47-120">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="63c47-121">クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントとデータ構造体のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="63c47-121">Represents a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="63c47-122">備考</span><span class="sxs-lookup"><span data-stu-id="63c47-122">Remarks</span></span>

<span data-ttu-id="63c47-123">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="63c47-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63c47-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="63c47-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63c47-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="63c47-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="63c47-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="63c47-126">Schema Name</span></span>  <br/> |<span data-ttu-id="63c47-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="63c47-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="63c47-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="63c47-128">Validation File</span></span>  <br/> |<span data-ttu-id="63c47-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="63c47-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="63c47-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="63c47-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="63c47-131">False</span><span class="sxs-lookup"><span data-stu-id="63c47-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63c47-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="63c47-132">See also</span></span>

- [<span data-ttu-id="63c47-133">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="63c47-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="63c47-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="63c47-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

