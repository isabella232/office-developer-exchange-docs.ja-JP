---
title: AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65554e4c-c0d9-485e-9f01-ed1baa8280ab
description: AddImContactToGroup 要素は、既存のインスタントメッセージングの連絡先をインスタントメッセージンググループに追加する要求を定義します。
ms.openlocfilehash: b86b1cb69a1ebc7034e5a27047c14efbab7236ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459666"
---
# <a name="addimcontacttogroup"></a><span data-ttu-id="b1013-103">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="b1013-103">AddImContactToGroup</span></span>

<span data-ttu-id="b1013-104">**Addimcontacttogroup**要素は、既存のインスタントメッセージングの連絡先をインスタントメッセージンググループに追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="b1013-104">The **AddImContactToGroup** element defines a request to add an existing instant messaging contact to an instant messaging group.</span></span> 
  
```XML
<AddImContactToGroup>
   <ContactId/>
   <GroupId/>
</AddImContactToGroup>
```

 <span data-ttu-id="b1013-105">**AddImContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="b1013-105">**AddImContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b1013-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b1013-106">Attributes and elements</span></span>

<span data-ttu-id="b1013-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b1013-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1013-108">属性</span><span class="sxs-lookup"><span data-stu-id="b1013-108">Attributes</span></span>

<span data-ttu-id="b1013-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b1013-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b1013-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b1013-110">Child elements</span></span>

<span data-ttu-id="b1013-111">[ContactId](contactid.md)  | [GroupId](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="b1013-111">[ContactId](contactid.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b1013-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b1013-112">Parent elements</span></span>

<span data-ttu-id="b1013-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b1013-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b1013-114">注釈</span><span class="sxs-lookup"><span data-stu-id="b1013-114">Remarks</span></span>

<span data-ttu-id="b1013-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b1013-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b1013-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b1013-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b1013-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b1013-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b1013-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="b1013-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b1013-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b1013-119">Schema name</span></span>  <br/> |<span data-ttu-id="b1013-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b1013-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b1013-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b1013-121">Validation file</span></span>  <br/> |<span data-ttu-id="b1013-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b1013-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b1013-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b1013-123">Can be empty</span></span>  <br/> |<span data-ttu-id="b1013-124">false</span><span class="sxs-lookup"><span data-stu-id="b1013-124">false</span></span>  <br/> |
   

