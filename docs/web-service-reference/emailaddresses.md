---
title: EmailAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EmailAddresses
api_type:
- schema
ms.assetid: fd4d773c-f7dc-4a04-9025-e772d7a45fdf
description: EmailAddresses 要素は、連絡先の電子メールアドレスのコレクションを表します。
ms.openlocfilehash: 9d247f6159d621124ecdd9968ee468ed2b4fe84b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456179"
---
# <a name="emailaddresses"></a><span data-ttu-id="c8978-103">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="c8978-103">EmailAddresses</span></span>

<span data-ttu-id="c8978-104">**Emailaddresses**要素は、連絡先の電子メールアドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c8978-104">The **EmailAddresses** element represents a collection of e-mail addresses for a contact.</span></span> 
  
```xml
<EmailAddresses>
   <Entry/>
</EmailAddresses>
```

 <span data-ttu-id="c8978-105">**EmailAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="c8978-105">**EmailAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8978-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c8978-106">Attributes and elements</span></span>

<span data-ttu-id="c8978-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c8978-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8978-108">属性</span><span class="sxs-lookup"><span data-stu-id="c8978-108">Attributes</span></span>

<span data-ttu-id="c8978-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c8978-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8978-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c8978-110">Child elements</span></span>

|<span data-ttu-id="c8978-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="c8978-111">**Element**</span></span>|<span data-ttu-id="c8978-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c8978-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8978-113">Entry (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="c8978-113">Entry (EmailAddress)</span></span>](entry-emailaddress.md) <br/> |<span data-ttu-id="c8978-114">連絡先の1つの電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="c8978-114">Represents a single e-mail address for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c8978-115">親要素</span><span class="sxs-lookup"><span data-stu-id="c8978-115">Parent elements</span></span>

|<span data-ttu-id="c8978-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="c8978-116">**Element**</span></span>|<span data-ttu-id="c8978-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c8978-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8978-118">連絡先</span><span class="sxs-lookup"><span data-stu-id="c8978-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c8978-119">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c8978-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c8978-120">注釈</span><span class="sxs-lookup"><span data-stu-id="c8978-120">Remarks</span></span>

<span data-ttu-id="c8978-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c8978-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8978-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c8978-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8978-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="c8978-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c8978-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c8978-124">Schema name</span></span>  <br/> |<span data-ttu-id="c8978-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c8978-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c8978-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c8978-126">Validation file</span></span>  <br/> |<span data-ttu-id="c8978-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c8978-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c8978-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c8978-128">Can be empty</span></span>  <br/> |<span data-ttu-id="c8978-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="c8978-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c8978-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="c8978-130">See also</span></span>

- [<span data-ttu-id="c8978-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c8978-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="c8978-132">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="c8978-132">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [<span data-ttu-id="c8978-133">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="c8978-133">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx) 
- [<span data-ttu-id="c8978-134">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="c8978-134">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

