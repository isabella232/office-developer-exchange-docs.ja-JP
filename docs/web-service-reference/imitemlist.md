---
title: ImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 556457d5-a730-4131-853f-1198c27c5942
description: ImItemList 要素には、インスタントメッセージンググループとインスタントメッセージングの連絡先の一覧が含まれています。
ms.openlocfilehash: 976897fd999b61207a94a8b1dc60cc1b1308acd8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460674"
---
# <a name="imitemlist"></a><span data-ttu-id="b2af9-103">ImItemList</span><span class="sxs-lookup"><span data-stu-id="b2af9-103">ImItemList</span></span>

<span data-ttu-id="b2af9-104">**Imitemlist**要素には、インスタントメッセージンググループとインスタントメッセージングの連絡先の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b2af9-104">The **ImItemList** element contains a list of instant messaging groups and instant messaging contacts.</span></span> 
  
```XML
<ImItemList>
   <Groups/>
   <Personas/>
</ImItemList>
```

 <span data-ttu-id="b2af9-105">**ImItemListType**</span><span class="sxs-lookup"><span data-stu-id="b2af9-105">**ImItemListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b2af9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b2af9-106">Attributes and elements</span></span>

<span data-ttu-id="b2af9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b2af9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2af9-108">属性</span><span class="sxs-lookup"><span data-stu-id="b2af9-108">Attributes</span></span>

<span data-ttu-id="b2af9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b2af9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2af9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b2af9-110">Child elements</span></span>

<span data-ttu-id="b2af9-111">[グループ (ArrayOfImGroupType)](groups-arrayofimgrouptype.md)  | [ペルソナ](personas-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="b2af9-111">[Groups (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [Personas](personas-ex15websvcsotherref.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b2af9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b2af9-112">Parent elements</span></span>

<span data-ttu-id="b2af9-113">[Getimitemsresponse](getimitemsresponse.md)  | [Getimitemlistresponse](getimitemlistresponse.md)</span><span class="sxs-lookup"><span data-stu-id="b2af9-113">[GetImItemsResponse](getimitemsresponse.md) | [GetImItemListResponse](getimitemlistresponse.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b2af9-114">注釈</span><span class="sxs-lookup"><span data-stu-id="b2af9-114">Remarks</span></span>

<span data-ttu-id="b2af9-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b2af9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b2af9-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b2af9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2af9-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b2af9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2af9-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="b2af9-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b2af9-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b2af9-119">Schema name</span></span>  <br/> |<span data-ttu-id="b2af9-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b2af9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b2af9-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b2af9-121">Validation file</span></span>  <br/> |<span data-ttu-id="b2af9-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b2af9-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b2af9-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b2af9-123">Can be empty</span></span>  <br/> ||
   

