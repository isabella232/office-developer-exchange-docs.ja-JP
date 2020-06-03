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
description: EncryptedSharedFolderData 要素には、クライアントが他のクライアントと予定表または連絡先データの共有を承認するために使用できる暗号化されたデータが含まれています。
ms.openlocfilehash: 52e91eaf1ded31602b11e50c1b62159f72c101cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530664"
---
# <a name="encryptedsharedfolderdata"></a><span data-ttu-id="7cc92-103">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="7cc92-103">EncryptedSharedFolderData</span></span>

<span data-ttu-id="7cc92-104">**Encryptedsharedfolderdata**要素には、クライアントが他のクライアントと予定表または連絡先データの共有を承認するために使用できる暗号化されたデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7cc92-104">The **EncryptedSharedFolderData** element contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 <span data-ttu-id="7cc92-105">**EncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="7cc92-105">**EncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7cc92-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7cc92-106">Attributes and elements</span></span>

<span data-ttu-id="7cc92-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7cc92-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cc92-108">属性</span><span class="sxs-lookup"><span data-stu-id="7cc92-108">Attributes</span></span>

<span data-ttu-id="7cc92-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7cc92-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7cc92-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7cc92-110">Child elements</span></span>

|<span data-ttu-id="7cc92-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7cc92-111">**Element**</span></span>|<span data-ttu-id="7cc92-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7cc92-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cc92-113">トークン</span><span class="sxs-lookup"><span data-stu-id="7cc92-113">Token</span></span>](token.md) <br/> |<span data-ttu-id="7cc92-114">共有データの識別トークンを表す暗号化されたデータを格納します。</span><span class="sxs-lookup"><span data-stu-id="7cc92-114">Contains encrypted data that represents the identification token for the shared data.</span></span>  <br/> |
|[<span data-ttu-id="7cc92-115">Data</span><span class="sxs-lookup"><span data-stu-id="7cc92-115">Data</span></span>](data.md) <br/> |<span data-ttu-id="7cc92-116">共有データを表す暗号化されたデータを格納します。</span><span class="sxs-lookup"><span data-stu-id="7cc92-116">Contains encrypted data that represents the shared data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7cc92-117">親要素</span><span class="sxs-lookup"><span data-stu-id="7cc92-117">Parent elements</span></span>

|<span data-ttu-id="7cc92-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="7cc92-118">**Element**</span></span>|<span data-ttu-id="7cc92-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="7cc92-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cc92-120">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="7cc92-120">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="7cc92-121">他のクライアントとの予定表または連絡先データの共有を承認するためにクライアントが使用できるデータ構造のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="7cc92-121">Represents a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7cc92-122">注釈</span><span class="sxs-lookup"><span data-stu-id="7cc92-122">Remarks</span></span>

<span data-ttu-id="7cc92-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7cc92-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7cc92-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7cc92-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7cc92-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="7cc92-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7cc92-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7cc92-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7cc92-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7cc92-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="7cc92-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7cc92-128">Validation File</span></span>  <br/> |<span data-ttu-id="7cc92-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7cc92-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7cc92-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7cc92-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7cc92-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="7cc92-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7cc92-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="7cc92-132">See also</span></span>

- [<span data-ttu-id="7cc92-133">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="7cc92-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="7cc92-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7cc92-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

