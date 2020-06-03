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
description: ProtocolConnection 要素は、サーバー Web クライアントのプロトコル接続を表します。
ms.openlocfilehash: b9df3febe36db53d7c5bf0610ba857f13aa96abc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528861"
---
# <a name="protocolconnection-soap"></a><span data-ttu-id="7a9ff-103">ProtocolConnection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7a9ff-103">ProtocolConnection (SOAP)</span></span>

<span data-ttu-id="7a9ff-104">**Protocolconnection**要素は、サーバー Web クライアントのプロトコル接続を表します。</span><span class="sxs-lookup"><span data-stu-id="7a9ff-104">The **ProtocolConnection** element represents the protocol connection of the server Web client.</span></span> 
  
```XML
<ProtocolConnection>
   <Hostname/>
   <Port/>
   <EncryptionMethod/>
</ProtocolConnection>
```

 <span data-ttu-id="7a9ff-105">**ProtocolConnection**</span><span class="sxs-lookup"><span data-stu-id="7a9ff-105">**ProtocolConnection**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a9ff-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7a9ff-106">Attributes and elements</span></span>

<span data-ttu-id="7a9ff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7a9ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a9ff-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a9ff-108">Attributes</span></span>

<span data-ttu-id="7a9ff-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7a9ff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a9ff-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7a9ff-110">Child elements</span></span>

|<span data-ttu-id="7a9ff-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7a9ff-111">**Element**</span></span>|<span data-ttu-id="7a9ff-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a9ff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a9ff-113">Hostname (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7a9ff-113">Hostname (SOAP)</span></span>](hostname-soap.md) <br/> |<span data-ttu-id="7a9ff-114">コンピューターの完全なコンピューター名のホスト名部分を表します。</span><span class="sxs-lookup"><span data-stu-id="7a9ff-114">Represents the host name portion of the full computer name of the computer.</span></span>  <br/> |
|[<span data-ttu-id="7a9ff-115">ポート (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7a9ff-115">Port (SOAP)</span></span>](port-soap.md) <br/> |<span data-ttu-id="7a9ff-116">プロトコルに使用するポート番号を表します。</span><span class="sxs-lookup"><span data-stu-id="7a9ff-116">Represents the port number to use for the protocol.</span></span>  <br/> |
|[<span data-ttu-id="7a9ff-117">EncryptionMethod (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7a9ff-117">EncryptionMethod (SOAP)</span></span>](encryptionmethod-soap.md) <br/> |<span data-ttu-id="7a9ff-118">POP、IMAP、および SMTP プロトコルに使用される暗号化方式を表します。</span><span class="sxs-lookup"><span data-stu-id="7a9ff-118">Represents the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a9ff-119">親要素</span><span class="sxs-lookup"><span data-stu-id="7a9ff-119">Parent elements</span></span>

|<span data-ttu-id="7a9ff-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="7a9ff-120">**Element**</span></span>|<span data-ttu-id="7a9ff-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a9ff-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a9ff-122">ProtocolConnections (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7a9ff-122">ProtocolConnections (SOAP)</span></span>](protocolconnections-soap.md) <br/> |<span data-ttu-id="7a9ff-123">0個以上のプロトコル接続を含みます。</span><span class="sxs-lookup"><span data-stu-id="7a9ff-123">Contains zero or more protocol connections.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7a9ff-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7a9ff-124">Text value</span></span>

<span data-ttu-id="7a9ff-125">なし。</span><span class="sxs-lookup"><span data-stu-id="7a9ff-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a9ff-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7a9ff-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a9ff-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="7a9ff-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="7a9ff-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7a9ff-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7a9ff-129">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="7a9ff-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="7a9ff-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7a9ff-130">Validation File</span></span>  <br/> |<span data-ttu-id="7a9ff-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7a9ff-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7a9ff-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7a9ff-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a9ff-133">正しい</span><span class="sxs-lookup"><span data-stu-id="7a9ff-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a9ff-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="7a9ff-134">See also</span></span>



[<span data-ttu-id="7a9ff-135">ProtocolConnectionCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7a9ff-135">ProtocolConnectionCollectionSetting (SOAP)</span></span>](protocolconnectioncollectionsetting-soap.md)

