---
title: EncryptionMethod (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bc632c85-ec74-4a00-baec-df5973e032fa
description: EncryptionMethod 要素は、POP、IMAP、および SMTP のプロトコルに使用される暗号化メソッドを表します。
ms.openlocfilehash: 5062d357a54019a576e391e1be4d4e8dfcc6e38d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760274"
---
# <a name="encryptionmethod-soap"></a><span data-ttu-id="261fe-103">EncryptionMethod (SOAP)</span><span class="sxs-lookup"><span data-stu-id="261fe-103">EncryptionMethod (SOAP)</span></span>

<span data-ttu-id="261fe-104">**EncryptionMethod**要素は、POP、IMAP、および SMTP のプロトコルに使用される暗号化メソッドを表します。</span><span class="sxs-lookup"><span data-stu-id="261fe-104">The **EncryptionMethod** element represents the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span> 
  
```XML
<EncryptionMethod/>
```

 <span data-ttu-id="261fe-105">**string**</span><span class="sxs-lookup"><span data-stu-id="261fe-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="261fe-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="261fe-106">Attributes and elements</span></span>

<span data-ttu-id="261fe-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="261fe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="261fe-108">属性</span><span class="sxs-lookup"><span data-stu-id="261fe-108">Attributes</span></span>

<span data-ttu-id="261fe-109">なし。</span><span class="sxs-lookup"><span data-stu-id="261fe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="261fe-110">子要素</span><span class="sxs-lookup"><span data-stu-id="261fe-110">Child elements</span></span>

<span data-ttu-id="261fe-111">なし。</span><span class="sxs-lookup"><span data-stu-id="261fe-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="261fe-112">親要素</span><span class="sxs-lookup"><span data-stu-id="261fe-112">Parent elements</span></span>

|<span data-ttu-id="261fe-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="261fe-113">**Element**</span></span>|<span data-ttu-id="261fe-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="261fe-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="261fe-115">ProtocolConnection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="261fe-115">ProtocolConnection (SOAP)</span></span>](protocolconnection-soap.md) <br/> |<span data-ttu-id="261fe-116">サーバーの Web クライアントのプロトコル接続を表します。</span><span class="sxs-lookup"><span data-stu-id="261fe-116">Represents the protocol connection of the server Web client.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="261fe-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="261fe-117">Text value</span></span>

<span data-ttu-id="261fe-118">この要素のテキスト値は、POP、IMAP、および SMTP のプロトコルに使用する暗号化方法です。</span><span class="sxs-lookup"><span data-stu-id="261fe-118">The text value for this element is the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="261fe-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="261fe-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="261fe-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="261fe-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="261fe-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="261fe-121">Schema Name</span></span>  <br/> |<span data-ttu-id="261fe-122">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="261fe-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="261fe-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="261fe-123">Validation File</span></span>  <br/> |<span data-ttu-id="261fe-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="261fe-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="261fe-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="261fe-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="261fe-126">True</span><span class="sxs-lookup"><span data-stu-id="261fe-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="261fe-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="261fe-127">See also</span></span>

- [<span data-ttu-id="261fe-128">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="261fe-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

