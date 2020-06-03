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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456179"
---
# <a name="emailaddresses"></a><span data-ttu-id="fcb82-103">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="fcb82-103">EmailAddresses</span></span>

<span data-ttu-id="fcb82-104">**Emailaddresses**要素は、連絡先の電子メールアドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="fcb82-104">The **EmailAddresses** element represents a collection of e-mail addresses for a contact.</span></span> 
  
```xml
<EmailAddresses>
   <Entry/>
</EmailAddresses>
```

 <span data-ttu-id="fcb82-105">**EmailAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="fcb82-105">**EmailAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fcb82-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fcb82-106">Attributes and elements</span></span>

<span data-ttu-id="fcb82-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fcb82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fcb82-108">属性</span><span class="sxs-lookup"><span data-stu-id="fcb82-108">Attributes</span></span>

<span data-ttu-id="fcb82-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fcb82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fcb82-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fcb82-110">Child elements</span></span>

|<span data-ttu-id="fcb82-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="fcb82-111">**Element**</span></span>|<span data-ttu-id="fcb82-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fcb82-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fcb82-113">Entry (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="fcb82-113">Entry (EmailAddress)</span></span>](entry-emailaddress.md) <br/> |<span data-ttu-id="fcb82-114">連絡先の1つの電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="fcb82-114">Represents a single e-mail address for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fcb82-115">親要素</span><span class="sxs-lookup"><span data-stu-id="fcb82-115">Parent elements</span></span>

|<span data-ttu-id="fcb82-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="fcb82-116">**Element**</span></span>|<span data-ttu-id="fcb82-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="fcb82-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fcb82-118">Contact</span><span class="sxs-lookup"><span data-stu-id="fcb82-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="fcb82-119">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="fcb82-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fcb82-120">注釈</span><span class="sxs-lookup"><span data-stu-id="fcb82-120">Remarks</span></span>

<span data-ttu-id="fcb82-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fcb82-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fcb82-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fcb82-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fcb82-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="fcb82-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fcb82-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fcb82-124">Schema name</span></span>  <br/> |<span data-ttu-id="fcb82-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="fcb82-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="fcb82-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fcb82-126">Validation file</span></span>  <br/> |<span data-ttu-id="fcb82-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="fcb82-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fcb82-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fcb82-128">Can be empty</span></span>  <br/> |<span data-ttu-id="fcb82-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="fcb82-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fcb82-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="fcb82-130">See also</span></span>

- [<span data-ttu-id="fcb82-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="fcb82-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="fcb82-132">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="fcb82-132">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [<span data-ttu-id="fcb82-133">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="fcb82-133">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx) 
- [<span data-ttu-id="fcb82-134">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="fcb82-134">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

