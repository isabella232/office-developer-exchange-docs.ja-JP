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
description: トークンの要素には、共有データの識別トークンを表す暗号化されたデータが含まれています。
ms.openlocfilehash: cec11d9f2c24a250483c5be6e273f981fdf0a8e6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839721"
---
# <a name="token"></a><span data-ttu-id="6d618-103">トークン</span><span class="sxs-lookup"><span data-stu-id="6d618-103">Token</span></span>

<span data-ttu-id="6d618-104">**トークン**の要素には、共有データの識別トークンを表す暗号化されたデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6d618-104">The **Token** element contains encrypted data that represents the identification token for the shared data.</span></span> 
  
```xml
<Token/>
```

 <span data-ttu-id="6d618-105">**EncryptedDataContainerType**</span><span class="sxs-lookup"><span data-stu-id="6d618-105">**EncryptedDataContainerType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d618-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6d618-106">Attributes and elements</span></span>

<span data-ttu-id="6d618-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6d618-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d618-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d618-108">Attributes</span></span>

<span data-ttu-id="6d618-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6d618-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d618-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6d618-110">Child elements</span></span>

<span data-ttu-id="6d618-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6d618-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6d618-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6d618-112">Parent elements</span></span>

|<span data-ttu-id="6d618-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6d618-113">**Element**</span></span>|<span data-ttu-id="6d618-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d618-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d618-115">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="6d618-115">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="6d618-116">クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントで暗号化されたデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6d618-116">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6d618-117">備考</span><span class="sxs-lookup"><span data-stu-id="6d618-117">Remarks</span></span>

<span data-ttu-id="6d618-118">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6d618-118">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d618-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="6d618-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d618-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="6d618-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6d618-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6d618-121">Schema Name</span></span>  <br/> |<span data-ttu-id="6d618-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6d618-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="6d618-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6d618-123">Validation File</span></span>  <br/> |<span data-ttu-id="6d618-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6d618-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d618-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6d618-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d618-126">False</span><span class="sxs-lookup"><span data-stu-id="6d618-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d618-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="6d618-127">See also</span></span>



[<span data-ttu-id="6d618-128">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="6d618-128">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="6d618-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6d618-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

