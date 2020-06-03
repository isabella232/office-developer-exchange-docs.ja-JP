---
title: 受信者 (ArrayOfSmtpAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipients
api_type:
- schema
ms.assetid: cf68417d-85cf-49e0-857a-f987d3675344
description: Recipients 要素は、メッセージの受信者の配列を指定します。
ms.openlocfilehash: 4c2478a81836c2e52baad9c928d112108679b837
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465507"
---
# <a name="recipients-arrayofsmtpaddresstype"></a><span data-ttu-id="f39da-103">受信者 (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="f39da-103">Recipients (ArrayOfSmtpAddressType)</span></span>

<span data-ttu-id="f39da-104">**Recipients**要素は、メッセージの受信者の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="f39da-104">The **Recipients** element specifies an array of recipients of a message.</span></span> 
  
```xml
<Recipients>   <SmtpAddress/></Recipients>
```

 <span data-ttu-id="f39da-105">**ArrayOfSmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="f39da-105">**ArrayOfSmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f39da-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f39da-106">Attributes and elements</span></span>

<span data-ttu-id="f39da-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f39da-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f39da-108">属性</span><span class="sxs-lookup"><span data-stu-id="f39da-108">Attributes</span></span>

<span data-ttu-id="f39da-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f39da-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f39da-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f39da-110">Child elements</span></span>

|<span data-ttu-id="f39da-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f39da-111">**Element**</span></span>|<span data-ttu-id="f39da-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f39da-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f39da-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="f39da-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="f39da-114">予定表または連絡先の共有要求の簡易メール転送プロトコル (SMTP) 受信者アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="f39da-114">Represents the Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f39da-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f39da-115">Parent elements</span></span>

|<span data-ttu-id="f39da-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="f39da-116">**Element**</span></span>|<span data-ttu-id="f39da-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="f39da-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f39da-118">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="f39da-118">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="f39da-119">共有への招待を識別する非透過の認証トークンを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f39da-119">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f39da-120">注釈</span><span class="sxs-lookup"><span data-stu-id="f39da-120">Remarks</span></span>

<span data-ttu-id="f39da-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f39da-121">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f39da-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f39da-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f39da-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="f39da-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f39da-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f39da-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f39da-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f39da-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f39da-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f39da-126">Validation File</span></span>  <br/> |<span data-ttu-id="f39da-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f39da-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f39da-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f39da-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="f39da-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="f39da-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f39da-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="f39da-130">See also</span></span>



[<span data-ttu-id="f39da-131">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="f39da-131">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="f39da-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f39da-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

