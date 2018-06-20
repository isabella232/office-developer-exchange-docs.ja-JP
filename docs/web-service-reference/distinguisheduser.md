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
description: DistinguishedUser 要素は、代理人アクセスの認証と既定のユーザー アカウントを識別します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: b14be22bfe5316b9ab254e63cdfa0757596b8b92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760131"
---
# <a name="distinguisheduser"></a><span data-ttu-id="58291-104">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="58291-104">DistinguishedUser</span></span>

<span data-ttu-id="58291-105">**DistinguishedUser**要素は、代理人アクセスの認証と既定のユーザー アカウントを識別します。</span><span class="sxs-lookup"><span data-stu-id="58291-105">The **DistinguishedUser** element identifies Anonymous and Default user accounts for delegate access.</span></span> <span data-ttu-id="58291-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="58291-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DistinguishedUser>Default or Anonymous</DistinguishedUser>
```

 <span data-ttu-id="58291-107">**DistinguishedUserType**</span><span class="sxs-lookup"><span data-stu-id="58291-107">**DistinguishedUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58291-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="58291-108">Attributes and elements</span></span>

<span data-ttu-id="58291-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="58291-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58291-110">属性</span><span class="sxs-lookup"><span data-stu-id="58291-110">Attributes</span></span>

<span data-ttu-id="58291-111">なし。</span><span class="sxs-lookup"><span data-stu-id="58291-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58291-112">子要素</span><span class="sxs-lookup"><span data-stu-id="58291-112">Child elements</span></span>

<span data-ttu-id="58291-113">なし。</span><span class="sxs-lookup"><span data-stu-id="58291-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="58291-114">親要素</span><span class="sxs-lookup"><span data-stu-id="58291-114">Parent elements</span></span>

|<span data-ttu-id="58291-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="58291-115">**Element**</span></span>|<span data-ttu-id="58291-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="58291-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58291-117">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="58291-117">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="58291-118">代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="58291-118">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="58291-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="58291-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="58291-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="58291-120">Text value</span></span>

<span data-ttu-id="58291-121">**既定**のテキスト値では、プリンシパルのメールボックスに追加されている代理人のユーザーの既定の設定について説明します。</span><span class="sxs-lookup"><span data-stu-id="58291-121">A text value of **Default** describes the default setting for delegate users who are added to the principal's mailbox.</span></span> <span data-ttu-id="58291-122">**匿名**のテキスト値では、匿名ユーザーがいる主体のメールボックスに代理人アクセスの設定について説明します。</span><span class="sxs-lookup"><span data-stu-id="58291-122">A text value of **Anonymous** describes the delegate access settings that anonymous users have on the principal's mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="58291-123">備考</span><span class="sxs-lookup"><span data-stu-id="58291-123">Remarks</span></span>

<span data-ttu-id="58291-124">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="58291-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58291-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="58291-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58291-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="58291-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58291-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="58291-127">Schema Name</span></span>  <br/> |<span data-ttu-id="58291-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="58291-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="58291-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="58291-129">Validation File</span></span>  <br/> |<span data-ttu-id="58291-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="58291-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="58291-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="58291-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="58291-132">False</span><span class="sxs-lookup"><span data-stu-id="58291-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58291-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="58291-133">See also</span></span>

- [<span data-ttu-id="58291-134">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="58291-134">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="58291-135">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="58291-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="58291-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="58291-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="58291-137">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="58291-137">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

