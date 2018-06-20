---
title: ProtocolConnection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6eef2188-6194-48f1-ad7e-46104aecdf56
description: ProtocolConnection 要素は、サーバーの Web クライアントのプロトコルの接続を表します。
ms.openlocfilehash: 8b5396821cd959e41d24fcf7a94c519f9c634a1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832915"
---
# <a name="protocolconnection-soap"></a><span data-ttu-id="b04ec-103">ProtocolConnection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b04ec-103">ProtocolConnection (SOAP)</span></span>

<span data-ttu-id="b04ec-104">**ProtocolConnection**要素は、サーバーの Web クライアントのプロトコルの接続を表します。</span><span class="sxs-lookup"><span data-stu-id="b04ec-104">The **ProtocolConnection** element represents the protocol connection of the server Web client.</span></span> 
  
```XML
<ProtocolConnection>
   <Hostname/>
   <Port/>
   <EncryptionMethod/>
</ProtocolConnection>
```

 <span data-ttu-id="b04ec-105">**ProtocolConnection**</span><span class="sxs-lookup"><span data-stu-id="b04ec-105">**ProtocolConnection**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b04ec-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b04ec-106">Attributes and elements</span></span>

<span data-ttu-id="b04ec-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b04ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b04ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="b04ec-108">Attributes</span></span>

<span data-ttu-id="b04ec-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b04ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b04ec-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b04ec-110">Child elements</span></span>

|<span data-ttu-id="b04ec-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b04ec-111">**Element**</span></span>|<span data-ttu-id="b04ec-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b04ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b04ec-113">ホスト名 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b04ec-113">Hostname (SOAP)</span></span>](hostname-soap.md) <br/> |<span data-ttu-id="b04ec-114">コンピューターのフル コンピューター名のホスト名の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="b04ec-114">Represents the host name portion of the full computer name of the computer.</span></span>  <br/> |
|[<span data-ttu-id="b04ec-115">ポート (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b04ec-115">Port (SOAP)</span></span>](port-soap.md) <br/> |<span data-ttu-id="b04ec-116">プロトコルに使用するポート番号を表します。</span><span class="sxs-lookup"><span data-stu-id="b04ec-116">Represents the port number to use for the protocol.</span></span>  <br/> |
|[<span data-ttu-id="b04ec-117">EncryptionMethod (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b04ec-117">EncryptionMethod (SOAP)</span></span>](encryptionmethod-soap.md) <br/> |<span data-ttu-id="b04ec-118">POP、IMAP、および SMTP のプロトコルに使用される暗号化メソッドを表します。</span><span class="sxs-lookup"><span data-stu-id="b04ec-118">Represents the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b04ec-119">親要素</span><span class="sxs-lookup"><span data-stu-id="b04ec-119">Parent elements</span></span>

|<span data-ttu-id="b04ec-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="b04ec-120">**Element**</span></span>|<span data-ttu-id="b04ec-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="b04ec-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b04ec-122">ProtocolConnections (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b04ec-122">ProtocolConnections (SOAP)</span></span>](protocolconnections-soap.md) <br/> |<span data-ttu-id="b04ec-123">0 個以上のプロトコルの接続が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b04ec-123">Contains zero or more protocol connections.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b04ec-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b04ec-124">Text value</span></span>

<span data-ttu-id="b04ec-125">なし。</span><span class="sxs-lookup"><span data-stu-id="b04ec-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b04ec-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="b04ec-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b04ec-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="b04ec-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="b04ec-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b04ec-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b04ec-129">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="b04ec-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="b04ec-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b04ec-130">Validation File</span></span>  <br/> |<span data-ttu-id="b04ec-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b04ec-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b04ec-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b04ec-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b04ec-133">True</span><span class="sxs-lookup"><span data-stu-id="b04ec-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b04ec-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b04ec-134">See also</span></span>



[<span data-ttu-id="b04ec-135">ProtocolConnectionCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b04ec-135">ProtocolConnectionCollectionSetting (SOAP)</span></span>](protocolconnectioncollectionsetting-soap.md)

