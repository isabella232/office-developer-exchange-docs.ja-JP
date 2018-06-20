---
title: ImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7b884e-ecf1-4e58-86ec-856b13a95f2b
description: ImGroup 要素は、インスタント メッセージングのグループを表します。
ms.openlocfilehash: 2a444158dbc6a73b1aee7b306cc251d33d005c43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831890"
---
# <a name="imgroup"></a><span data-ttu-id="15c9e-103">ImGroup</span><span class="sxs-lookup"><span data-stu-id="15c9e-103">ImGroup</span></span>

<span data-ttu-id="15c9e-104">**ImGroup**要素は、インスタント メッセージングのグループを表します。</span><span class="sxs-lookup"><span data-stu-id="15c9e-104">The **ImGroup** element represents an instant messaging group.</span></span> 
  
```XML
<ImGroup>
   <DisplayName/>
   <GroupType/>
   <ExchangeStoreId/>
   <MemberCorrelationKey/>
   <ExtendedProperties/>
   <SmtpAddress/>
</ImGroup>
```

 <span data-ttu-id="15c9e-105">**ImGroupType**</span><span class="sxs-lookup"><span data-stu-id="15c9e-105">**ImGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15c9e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="15c9e-106">Attributes and elements</span></span>

<span data-ttu-id="15c9e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="15c9e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15c9e-108">属性</span><span class="sxs-lookup"><span data-stu-id="15c9e-108">Attributes</span></span>

<span data-ttu-id="15c9e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="15c9e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15c9e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="15c9e-110">Child elements</span></span>

<span data-ttu-id="15c9e-111">[表示名 (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupType](grouptype.md) | [ExchangeStoreId](exchangestoreid.md) | [MemberCorrelationKey](membercorrelationkey.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)  |  [SmtpAddress](smtpaddress.md)</span><span class="sxs-lookup"><span data-stu-id="15c9e-111">[DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupType](grouptype.md) | [ExchangeStoreId](exchangestoreid.md) | [MemberCorrelationKey](membercorrelationkey.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md) | [SmtpAddress](smtpaddress.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="15c9e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="15c9e-112">Parent elements</span></span>

<span data-ttu-id="15c9e-113">[グループ (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md) | [AddImGroupResponse](addimgroupresponse.md)</span><span class="sxs-lookup"><span data-stu-id="15c9e-113">[Groups (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md) | [AddImGroupResponse](addimgroupresponse.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="15c9e-114">備考</span><span class="sxs-lookup"><span data-stu-id="15c9e-114">Remarks</span></span>

<span data-ttu-id="15c9e-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="15c9e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="15c9e-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="15c9e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15c9e-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="15c9e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15c9e-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="15c9e-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="15c9e-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="15c9e-119">Schema name</span></span>  <br/> |<span data-ttu-id="15c9e-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="15c9e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="15c9e-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="15c9e-121">Validation file</span></span>  <br/> |<span data-ttu-id="15c9e-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="15c9e-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="15c9e-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="15c9e-123">Can be empty</span></span>  <br/> ||
   

