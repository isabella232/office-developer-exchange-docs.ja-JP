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
description: SmtpAddress 要素では、偽装に使用するアカウントの簡易メール転送プロトコル (SMTP) アドレス、または予定表または連絡先の共有の依頼の簡易メール転送プロトコル (SMTP) 受信者のアドレスを表します。
ms.openlocfilehash: 39588f0892cdcec819a1972547155730be5785f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833511"
---
# <a name="smtpaddress"></a><span data-ttu-id="ef582-103">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="ef582-103">SmtpAddress</span></span>

<span data-ttu-id="ef582-104">**SmtpAddress**要素では、偽装に使用するアカウントの簡易メール転送プロトコル (SMTP) アドレス、または予定表または連絡先の共有の依頼の簡易メール転送プロトコル (SMTP) 受信者のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="ef582-104">The **SmtpAddress** element represents the Simple Mail Transfer Protocol (SMTP) address of an account to be used for impersonation or a Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span> 
  
```xml
<SmtpAddress/>
```

<span data-ttu-id="ef582-105">**SmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="ef582-105">**SmtpAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ef582-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ef582-106">Attributes and elements</span></span>

<span data-ttu-id="ef582-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ef582-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef582-108">属性</span><span class="sxs-lookup"><span data-stu-id="ef582-108">Attributes</span></span>

<span data-ttu-id="ef582-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ef582-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef582-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ef582-110">Child elements</span></span>

<span data-ttu-id="ef582-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ef582-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ef582-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ef582-112">Parent elements</span></span>

|<span data-ttu-id="ef582-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ef582-113">**Element**</span></span>|<span data-ttu-id="ef582-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ef582-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef582-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="ef582-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="ef582-116">ExchangeImpersonation SOAP ヘッダーを使用する際に偽装するアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="ef582-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="ef582-117">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="ef582-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="ef582-118">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="ef582-118">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="ef582-119">予定表の共有または共有メッセージを取引先担当者の無効な受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="ef582-119">Represents an invalid recipient for a calendar sharing or contact sharing message.</span></span>  <br/> |
|[<span data-ttu-id="ef582-120">受信者 (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="ef582-120">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="ef582-121">共有フォルダーへのアクセスを許可する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ef582-121">Represents a collection of recipients that will be granted access to the shared folder.</span></span>  <br/> |
|[<span data-ttu-id="ef582-122">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="ef582-122">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="ef582-123">指定した共有フォルダーのローカル フォルダーの識別子を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="ef582-123">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ef582-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ef582-124">Text value</span></span>

<span data-ttu-id="ef582-125">SMTP アドレスを表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef582-125">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ef582-126">備考</span><span class="sxs-lookup"><span data-stu-id="ef582-126">Remarks</span></span>

<span data-ttu-id="ef582-127">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ef582-127">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef582-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="ef582-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef582-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="ef582-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ef582-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ef582-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ef582-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ef582-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="ef582-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ef582-132">Validation File</span></span>  <br/> |<span data-ttu-id="ef582-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ef582-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ef582-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ef582-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef582-135">False</span><span class="sxs-lookup"><span data-stu-id="ef582-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef582-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="ef582-136">See also</span></span>

- [<span data-ttu-id="ef582-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ef582-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

