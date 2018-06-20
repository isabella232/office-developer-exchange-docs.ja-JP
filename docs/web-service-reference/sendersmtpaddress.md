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
description: SenderSmtpAddress 要素は、共有されるフォルダーを含むメールボックスに対応する SMTP 電子メール アドレスを表します。
ms.openlocfilehash: 70905dd1ae2c3df18224aceeea246b542d1338e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833334"
---
# <a name="sendersmtpaddress"></a><span data-ttu-id="d4b15-103">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="d4b15-103">SenderSmtpAddress</span></span>

<span data-ttu-id="d4b15-104">**SenderSmtpAddress**要素は、共有されるフォルダーを含むメールボックスに対応する SMTP 電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="d4b15-104">The **SenderSmtpAddress** element represents the SMTP e-mail address corresponding to the mailbox that contains the folder that will be shared.</span></span> 
  
```xml
<SenderSmtpAddress/>
```

 <span data-ttu-id="d4b15-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="d4b15-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4b15-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d4b15-106">Attributes and elements</span></span>

<span data-ttu-id="d4b15-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d4b15-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4b15-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4b15-108">Attributes</span></span>

<span data-ttu-id="d4b15-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d4b15-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4b15-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d4b15-110">Child elements</span></span>

<span data-ttu-id="d4b15-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d4b15-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4b15-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d4b15-112">Parent elements</span></span>

|<span data-ttu-id="d4b15-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d4b15-113">**Element**</span></span>|<span data-ttu-id="d4b15-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d4b15-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4b15-115">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="d4b15-115">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="d4b15-116">共有への招待を識別する不透明な認証トークンを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="d4b15-116">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d4b15-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d4b15-117">Text value</span></span>

<span data-ttu-id="d4b15-118">SMTP アドレスを表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4b15-118">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d4b15-119">備考</span><span class="sxs-lookup"><span data-stu-id="d4b15-119">Remarks</span></span>

<span data-ttu-id="d4b15-120">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d4b15-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4b15-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="d4b15-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4b15-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="d4b15-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d4b15-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d4b15-123">Schema Name</span></span>  <br/> |<span data-ttu-id="d4b15-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d4b15-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d4b15-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d4b15-125">Validation File</span></span>  <br/> |<span data-ttu-id="d4b15-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d4b15-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d4b15-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d4b15-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4b15-128">False</span><span class="sxs-lookup"><span data-stu-id="d4b15-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4b15-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="d4b15-129">See also</span></span>



[<span data-ttu-id="d4b15-130">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="d4b15-130">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="d4b15-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d4b15-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

