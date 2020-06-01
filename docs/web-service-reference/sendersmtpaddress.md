---
title: SenderSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderSmtpAddress
api_type:
- schema
ms.assetid: e39c7df7-4bfa-455f-b4bb-1f1d05398eec
description: SenderSmtpAddress 要素は、共有されるフォルダーが含まれているメールボックスに対応する SMTP 電子メールアドレスを表します。
ms.openlocfilehash: 73047dcecfbccb55d74e373891c3154bc7baeeba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464897"
---
# <a name="sendersmtpaddress"></a><span data-ttu-id="1dc25-103">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1dc25-103">SenderSmtpAddress</span></span>

<span data-ttu-id="1dc25-104">**SenderSmtpAddress**要素は、共有されるフォルダーが含まれているメールボックスに対応する SMTP 電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="1dc25-104">The **SenderSmtpAddress** element represents the SMTP e-mail address corresponding to the mailbox that contains the folder that will be shared.</span></span> 
  
```xml
<SenderSmtpAddress/>
```

 <span data-ttu-id="1dc25-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="1dc25-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1dc25-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1dc25-106">Attributes and elements</span></span>

<span data-ttu-id="1dc25-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1dc25-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1dc25-108">属性</span><span class="sxs-lookup"><span data-stu-id="1dc25-108">Attributes</span></span>

<span data-ttu-id="1dc25-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1dc25-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1dc25-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1dc25-110">Child elements</span></span>

<span data-ttu-id="1dc25-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1dc25-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1dc25-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1dc25-112">Parent elements</span></span>

|<span data-ttu-id="1dc25-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1dc25-113">**Element**</span></span>|<span data-ttu-id="1dc25-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1dc25-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dc25-115">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="1dc25-115">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="1dc25-116">共有への招待を識別する非透過の認証トークンを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="1dc25-116">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1dc25-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1dc25-117">Text value</span></span>

<span data-ttu-id="1dc25-118">SMTP アドレスを表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="1dc25-118">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1dc25-119">注釈</span><span class="sxs-lookup"><span data-stu-id="1dc25-119">Remarks</span></span>

<span data-ttu-id="1dc25-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1dc25-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1dc25-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1dc25-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1dc25-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="1dc25-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1dc25-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1dc25-123">Schema Name</span></span>  <br/> |<span data-ttu-id="1dc25-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1dc25-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1dc25-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1dc25-125">Validation File</span></span>  <br/> |<span data-ttu-id="1dc25-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1dc25-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1dc25-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1dc25-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="1dc25-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="1dc25-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1dc25-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="1dc25-129">See also</span></span>



[<span data-ttu-id="1dc25-130">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="1dc25-130">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="1dc25-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1dc25-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

