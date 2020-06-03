---
title: SmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SmtpAddress
api_type:
- schema
ms.assetid: 779305a6-ad1e-424e-8a69-4e3bef61d787
description: SmtpAddress 要素は、偽装に使用されるアカウントの簡易メール転送プロトコル (SMTP) アドレス、または予定表または連絡先共有要求の SMTP (Simple Mail Transfer Protocol) 受信者アドレスを表します。
ms.openlocfilehash: 915ff328cc384c1f2884e9fbea8c10c1ebc79288
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466690"
---
# <a name="smtpaddress"></a><span data-ttu-id="450e6-103">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="450e6-103">SmtpAddress</span></span>

<span data-ttu-id="450e6-104">**Smtpaddress**要素は、偽装に使用されるアカウントの簡易メール転送プロトコル (smtp) アドレス、または予定表または連絡先共有要求の Smtp (Simple Mail transfer protocol) 受信者アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="450e6-104">The **SmtpAddress** element represents the Simple Mail Transfer Protocol (SMTP) address of an account to be used for impersonation or a Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span> 
  
```xml
<SmtpAddress/>
```

<span data-ttu-id="450e6-105">**SmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="450e6-105">**SmtpAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="450e6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="450e6-106">Attributes and elements</span></span>

<span data-ttu-id="450e6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="450e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="450e6-108">属性</span><span class="sxs-lookup"><span data-stu-id="450e6-108">Attributes</span></span>

<span data-ttu-id="450e6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="450e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="450e6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="450e6-110">Child elements</span></span>

<span data-ttu-id="450e6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="450e6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="450e6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="450e6-112">Parent elements</span></span>

|<span data-ttu-id="450e6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="450e6-113">**Element**</span></span>|<span data-ttu-id="450e6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="450e6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="450e6-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="450e6-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="450e6-116">ExchangeImpersonation SOAP ヘッダーを使用しているときに偽装するアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="450e6-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="450e6-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="450e6-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="450e6-118">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="450e6-118">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="450e6-119">予定表共有または連絡先共有メッセージの無効な受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="450e6-119">Represents an invalid recipient for a calendar sharing or contact sharing message.</span></span>  <br/> |
|[<span data-ttu-id="450e6-120">受信者 (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="450e6-120">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="450e6-121">共有フォルダーへのアクセスが許可される受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="450e6-121">Represents a collection of recipients that will be granted access to the shared folder.</span></span>  <br/> |
|[<span data-ttu-id="450e6-122">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="450e6-122">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="450e6-123">指定された共有フォルダーのローカルフォルダー識別子を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="450e6-123">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="450e6-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="450e6-124">Text value</span></span>

<span data-ttu-id="450e6-125">SMTP アドレスを表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="450e6-125">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="450e6-126">注釈</span><span class="sxs-lookup"><span data-stu-id="450e6-126">Remarks</span></span>

<span data-ttu-id="450e6-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="450e6-127">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="450e6-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="450e6-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="450e6-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="450e6-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="450e6-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="450e6-130">Schema Name</span></span>  <br/> |<span data-ttu-id="450e6-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="450e6-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="450e6-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="450e6-132">Validation File</span></span>  <br/> |<span data-ttu-id="450e6-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="450e6-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="450e6-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="450e6-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="450e6-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="450e6-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="450e6-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="450e6-136">See also</span></span>

- [<span data-ttu-id="450e6-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="450e6-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

