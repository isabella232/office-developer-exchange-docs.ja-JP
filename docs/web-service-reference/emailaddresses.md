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
description: EmailAddresses 要素は、連絡先の電子メール アドレスのコレクションを表します。
ms.openlocfilehash: 2eddb68ecffd8f61a2fbb775d8013433d715db1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760235"
---
# <a name="emailaddresses"></a><span data-ttu-id="70970-103">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="70970-103">EmailAddresses</span></span>

<span data-ttu-id="70970-104">**EmailAddresses**要素は、連絡先の電子メール アドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="70970-104">The **EmailAddresses** element represents a collection of e-mail addresses for a contact.</span></span> 
  
```xml
<EmailAddresses>
   <Entry/>
</EmailAddresses>
```

 <span data-ttu-id="70970-105">**EmailAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="70970-105">**EmailAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70970-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="70970-106">Attributes and elements</span></span>

<span data-ttu-id="70970-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="70970-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70970-108">属性</span><span class="sxs-lookup"><span data-stu-id="70970-108">Attributes</span></span>

<span data-ttu-id="70970-109">なし。</span><span class="sxs-lookup"><span data-stu-id="70970-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70970-110">子要素</span><span class="sxs-lookup"><span data-stu-id="70970-110">Child elements</span></span>

|<span data-ttu-id="70970-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="70970-111">**Element**</span></span>|<span data-ttu-id="70970-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="70970-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70970-113">エントリ (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="70970-113">Entry (EmailAddress)</span></span>](entry-emailaddress.md) <br/> |<span data-ttu-id="70970-114">連絡先の単一の電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="70970-114">Represents a single e-mail address for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="70970-115">親要素</span><span class="sxs-lookup"><span data-stu-id="70970-115">Parent elements</span></span>

|<span data-ttu-id="70970-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="70970-116">**Element**</span></span>|<span data-ttu-id="70970-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="70970-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70970-118">Contact</span><span class="sxs-lookup"><span data-stu-id="70970-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="70970-119">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="70970-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="70970-120">備考</span><span class="sxs-lookup"><span data-stu-id="70970-120">Remarks</span></span>

<span data-ttu-id="70970-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="70970-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70970-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="70970-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70970-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="70970-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="70970-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="70970-124">Schema name</span></span>  <br/> |<span data-ttu-id="70970-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="70970-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="70970-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="70970-126">Validation file</span></span>  <br/> |<span data-ttu-id="70970-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="70970-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="70970-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="70970-128">Can be empty</span></span>  <br/> |<span data-ttu-id="70970-129">False</span><span class="sxs-lookup"><span data-stu-id="70970-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70970-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="70970-130">See also</span></span>

- [<span data-ttu-id="70970-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="70970-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="70970-132">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="70970-132">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [<span data-ttu-id="70970-133">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="70970-133">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx) 
- [<span data-ttu-id="70970-134">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="70970-134">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

