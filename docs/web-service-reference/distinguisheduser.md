---
title: DistinguishedUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedUser
api_type:
- schema
ms.assetid: 9362699d-666a-4acf-8fa1-c6669f0a2ae5
description: DistinguishedUser 要素は、代理人アクセスの匿名および既定のユーザーアカウントを識別します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 922c36251290d7090cdafbed9e570144593ca97e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530734"
---
# <a name="distinguisheduser"></a><span data-ttu-id="12e65-104">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="12e65-104">DistinguishedUser</span></span>

<span data-ttu-id="12e65-105">**DistinguishedUser**要素は、代理人アクセスの匿名および既定のユーザーアカウントを識別します。</span><span class="sxs-lookup"><span data-stu-id="12e65-105">The **DistinguishedUser** element identifies Anonymous and Default user accounts for delegate access.</span></span> <span data-ttu-id="12e65-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="12e65-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DistinguishedUser>Default or Anonymous</DistinguishedUser>
```

 <span data-ttu-id="12e65-107">**DistinguishedUserType**</span><span class="sxs-lookup"><span data-stu-id="12e65-107">**DistinguishedUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12e65-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="12e65-108">Attributes and elements</span></span>

<span data-ttu-id="12e65-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="12e65-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12e65-110">属性</span><span class="sxs-lookup"><span data-stu-id="12e65-110">Attributes</span></span>

<span data-ttu-id="12e65-111">なし。</span><span class="sxs-lookup"><span data-stu-id="12e65-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12e65-112">子要素</span><span class="sxs-lookup"><span data-stu-id="12e65-112">Child elements</span></span>

<span data-ttu-id="12e65-113">なし。</span><span class="sxs-lookup"><span data-stu-id="12e65-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="12e65-114">親要素</span><span class="sxs-lookup"><span data-stu-id="12e65-114">Parent elements</span></span>

|<span data-ttu-id="12e65-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="12e65-115">**Element**</span></span>|<span data-ttu-id="12e65-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="12e65-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12e65-117">UserId</span><span class="sxs-lookup"><span data-stu-id="12e65-117">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="12e65-118">代理ユーザーまたはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="12e65-118">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="12e65-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="12e65-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12e65-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="12e65-120">Text value</span></span>

<span data-ttu-id="12e65-121">**既定**のテキスト値は、プリンシパルのメールボックスに追加された代理人ユーザーの既定の設定を示します。</span><span class="sxs-lookup"><span data-stu-id="12e65-121">A text value of **Default** describes the default setting for delegate users who are added to the principal's mailbox.</span></span> <span data-ttu-id="12e65-122">**Anonymous**のテキスト値は、匿名ユーザーがプリンシパルのメールボックスに対して持っている代理人アクセス設定について説明します。</span><span class="sxs-lookup"><span data-stu-id="12e65-122">A text value of **Anonymous** describes the delegate access settings that anonymous users have on the principal's mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="12e65-123">注釈</span><span class="sxs-lookup"><span data-stu-id="12e65-123">Remarks</span></span>

<span data-ttu-id="12e65-124">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="12e65-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12e65-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="12e65-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12e65-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="12e65-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12e65-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="12e65-127">Schema Name</span></span>  <br/> |<span data-ttu-id="12e65-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="12e65-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="12e65-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="12e65-129">Validation File</span></span>  <br/> |<span data-ttu-id="12e65-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="12e65-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12e65-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="12e65-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="12e65-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="12e65-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12e65-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="12e65-133">See also</span></span>

- [<span data-ttu-id="12e65-134">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="12e65-134">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="12e65-135">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="12e65-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="12e65-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="12e65-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="12e65-137">代理人の追加</span><span class="sxs-lookup"><span data-stu-id="12e65-137">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

