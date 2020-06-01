---
title: トークン
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Token
api_type:
- schema
ms.assetid: 62b700e1-88c7-41ef-b431-d7af4a8b54a7
description: Token 要素には、共有データの識別トークンを表す暗号化されたデータが含まれています。
ms.openlocfilehash: c2e80082f9b4ecb96defdca8c5f0223a945661ba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458909"
---
# <a name="token"></a><span data-ttu-id="6fe36-103">トークン</span><span class="sxs-lookup"><span data-stu-id="6fe36-103">Token</span></span>

<span data-ttu-id="6fe36-104">**Token**要素には、共有データの識別トークンを表す暗号化されたデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6fe36-104">The **Token** element contains encrypted data that represents the identification token for the shared data.</span></span> 
  
```xml
<Token/>
```

 <span data-ttu-id="6fe36-105">**EncryptedDataContainerType**</span><span class="sxs-lookup"><span data-stu-id="6fe36-105">**EncryptedDataContainerType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6fe36-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6fe36-106">Attributes and elements</span></span>

<span data-ttu-id="6fe36-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6fe36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6fe36-108">属性</span><span class="sxs-lookup"><span data-stu-id="6fe36-108">Attributes</span></span>

<span data-ttu-id="6fe36-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6fe36-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6fe36-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6fe36-110">Child elements</span></span>

<span data-ttu-id="6fe36-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6fe36-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6fe36-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6fe36-112">Parent elements</span></span>

|<span data-ttu-id="6fe36-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6fe36-113">**Element**</span></span>|<span data-ttu-id="6fe36-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6fe36-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fe36-115">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="6fe36-115">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="6fe36-116">クライアントが他のクライアントと予定表または連絡先データの共有を承認するために使用できる暗号化されたデータを格納します。</span><span class="sxs-lookup"><span data-stu-id="6fe36-116">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6fe36-117">注釈</span><span class="sxs-lookup"><span data-stu-id="6fe36-117">Remarks</span></span>

<span data-ttu-id="6fe36-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6fe36-118">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6fe36-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6fe36-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6fe36-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="6fe36-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6fe36-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6fe36-121">Schema Name</span></span>  <br/> |<span data-ttu-id="6fe36-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6fe36-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="6fe36-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6fe36-123">Validation File</span></span>  <br/> |<span data-ttu-id="6fe36-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6fe36-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6fe36-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6fe36-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="6fe36-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="6fe36-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6fe36-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="6fe36-127">See also</span></span>



[<span data-ttu-id="6fe36-128">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="6fe36-128">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="6fe36-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6fe36-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

