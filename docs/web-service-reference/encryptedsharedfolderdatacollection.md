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
description: EncryptedSharedFolderDataCollection 要素には、他のクライアントとの予定表または連絡先データの共有を承認するためにクライアントが使用できるデータ構造のコレクションが含まれています。
ms.openlocfilehash: e8ed9221952892abda7b4eac62b16cdc4976c6e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461269"
---
# <a name="encryptedsharedfolderdatacollection"></a><span data-ttu-id="b0be8-103">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="b0be8-103">EncryptedSharedFolderDataCollection</span></span>

<span data-ttu-id="b0be8-104">**EncryptedSharedFolderDataCollection**要素には、他のクライアントとの予定表または連絡先データの共有を承認するためにクライアントが使用できるデータ構造のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0be8-104">The **EncryptedSharedFolderDataCollection** element contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderDataCollection>   <EncryptedSharedFolderData/></EncryptedSharedFolderDataCollection>
```

 <span data-ttu-id="b0be8-105">**ArrayOfEncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="b0be8-105">**ArrayOfEncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0be8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b0be8-106">Attributes and elements</span></span>

<span data-ttu-id="b0be8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b0be8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0be8-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0be8-108">Attributes</span></span>

<span data-ttu-id="b0be8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b0be8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0be8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b0be8-110">Child elements</span></span>

|<span data-ttu-id="b0be8-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="b0be8-111">**Element**</span></span>|<span data-ttu-id="b0be8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0be8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0be8-113">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="b0be8-113">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="b0be8-114">クライアントが他のクライアントと予定表または連絡先データの共有を承認するために使用できる暗号化されたデータを格納します。</span><span class="sxs-lookup"><span data-stu-id="b0be8-114">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0be8-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b0be8-115">Parent elements</span></span>

|<span data-ttu-id="b0be8-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="b0be8-116">**Element**</span></span>|<span data-ttu-id="b0be8-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0be8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0be8-118">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="b0be8-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="b0be8-119">[Getsharingmetadata 操作](getsharingmetadata-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="b0be8-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="b0be8-120">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b0be8-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="b0be8-121">1つの[Getsharingmetadata 操作](getsharingmetadata-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="b0be8-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b0be8-122">注釈</span><span class="sxs-lookup"><span data-stu-id="b0be8-122">Remarks</span></span>

<span data-ttu-id="b0be8-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b0be8-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0be8-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b0be8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0be8-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="b0be8-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b0be8-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b0be8-126">Schema Name</span></span>  <br/> |<span data-ttu-id="b0be8-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b0be8-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b0be8-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b0be8-128">Validation File</span></span>  <br/> |<span data-ttu-id="b0be8-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b0be8-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b0be8-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b0be8-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0be8-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="b0be8-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0be8-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0be8-132">See also</span></span>

- [<span data-ttu-id="b0be8-133">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="b0be8-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="b0be8-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b0be8-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

