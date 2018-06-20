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
description: 宛先の要素は、メッセージの受信者の配列を指定します。
ms.openlocfilehash: 8490988043b1e06fd3a8f553fcefaeb2e90e9d31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832988"
---
# <a name="recipients-arrayofsmtpaddresstype"></a><span data-ttu-id="d7329-103">受信者 (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="d7329-103">Recipients (ArrayOfSmtpAddressType)</span></span>

<span data-ttu-id="d7329-104">**宛先**の要素は、メッセージの受信者の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="d7329-104">The **Recipients** element specifies an array of recipients of a message.</span></span> 
  
```xml
<Recipients>   <SmtpAddress/></Recipients>
```

 <span data-ttu-id="d7329-105">**ArrayOfSmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="d7329-105">**ArrayOfSmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7329-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d7329-106">Attributes and elements</span></span>

<span data-ttu-id="d7329-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d7329-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7329-108">属性</span><span class="sxs-lookup"><span data-stu-id="d7329-108">Attributes</span></span>

<span data-ttu-id="d7329-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d7329-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7329-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d7329-110">Child elements</span></span>

|<span data-ttu-id="d7329-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d7329-111">**Element**</span></span>|<span data-ttu-id="d7329-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d7329-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7329-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="d7329-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="d7329-114">予定表または連絡先の共有の依頼の受信者の簡易メール転送プロトコル (SMTP) アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="d7329-114">Represents the Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d7329-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d7329-115">Parent elements</span></span>

|<span data-ttu-id="d7329-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d7329-116">**Element**</span></span>|<span data-ttu-id="d7329-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d7329-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7329-118">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="d7329-118">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="d7329-119">共有への招待を識別する不透明な認証トークンを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="d7329-119">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d7329-120">備考</span><span class="sxs-lookup"><span data-stu-id="d7329-120">Remarks</span></span>

<span data-ttu-id="d7329-121">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d7329-121">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7329-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="d7329-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7329-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="d7329-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d7329-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d7329-124">Schema Name</span></span>  <br/> |<span data-ttu-id="d7329-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d7329-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d7329-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d7329-126">Validation File</span></span>  <br/> |<span data-ttu-id="d7329-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d7329-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d7329-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d7329-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7329-129">False</span><span class="sxs-lookup"><span data-stu-id="d7329-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7329-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d7329-130">See also</span></span>



[<span data-ttu-id="d7329-131">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="d7329-131">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="d7329-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d7329-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

