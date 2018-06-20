---
title: ImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 556457d5-a730-4131-853f-1198c27c5942
description: ImItemList 要素には、インスタント メッセージング グループとインスタント メッセージングのメンバーの一覧が含まれています。
ms.openlocfilehash: 490ac57da0c7ae7bedc75e94b7e21dc30c9da23f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831896"
---
# <a name="imitemlist"></a><span data-ttu-id="be694-103">ImItemList</span><span class="sxs-lookup"><span data-stu-id="be694-103">ImItemList</span></span>

<span data-ttu-id="be694-104">**ImItemList**要素には、インスタント メッセージング グループとインスタント メッセージングのメンバーの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="be694-104">The **ImItemList** element contains a list of instant messaging groups and instant messaging contacts.</span></span> 
  
```XML
<ImItemList>
   <Groups/>
   <Personas/>
</ImItemList>
```

 <span data-ttu-id="be694-105">**ImItemListType**</span><span class="sxs-lookup"><span data-stu-id="be694-105">**ImItemListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be694-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="be694-106">Attributes and elements</span></span>

<span data-ttu-id="be694-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="be694-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be694-108">属性</span><span class="sxs-lookup"><span data-stu-id="be694-108">Attributes</span></span>

<span data-ttu-id="be694-109">なし。</span><span class="sxs-lookup"><span data-stu-id="be694-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="be694-110">子要素</span><span class="sxs-lookup"><span data-stu-id="be694-110">Child elements</span></span>

<span data-ttu-id="be694-111">[グループ (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [ペルソナ](personas-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="be694-111">[Groups (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [Personas](personas-ex15websvcsotherref.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="be694-112">親要素</span><span class="sxs-lookup"><span data-stu-id="be694-112">Parent elements</span></span>

<span data-ttu-id="be694-113">[GetImItemsResponse](getimitemsresponse.md) | [GetImItemListResponse](getimitemlistresponse.md)</span><span class="sxs-lookup"><span data-stu-id="be694-113">[GetImItemsResponse](getimitemsresponse.md) | [GetImItemListResponse](getimitemlistresponse.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="be694-114">備考</span><span class="sxs-lookup"><span data-stu-id="be694-114">Remarks</span></span>

<span data-ttu-id="be694-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="be694-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="be694-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="be694-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be694-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="be694-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be694-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="be694-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="be694-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="be694-119">Schema name</span></span>  <br/> |<span data-ttu-id="be694-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="be694-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="be694-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="be694-121">Validation file</span></span>  <br/> |<span data-ttu-id="be694-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="be694-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="be694-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="be694-123">Can be empty</span></span>  <br/> ||
   

