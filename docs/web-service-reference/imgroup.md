---
title: ImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7b884e-ecf1-4e58-86ec-856b13a95f2b
description: ImGroup 要素は、インスタントメッセージンググループを表します。
ms.openlocfilehash: a0ff3fcb82e7f18837af5a6f5daa16e90043034d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460688"
---
# <a name="imgroup"></a><span data-ttu-id="f9cad-103">ImGroup</span><span class="sxs-lookup"><span data-stu-id="f9cad-103">ImGroup</span></span>

<span data-ttu-id="f9cad-104">**Imgroup**要素は、インスタントメッセージンググループを表します。</span><span class="sxs-lookup"><span data-stu-id="f9cad-104">The **ImGroup** element represents an instant messaging group.</span></span> 
  
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

 <span data-ttu-id="f9cad-105">**ImGroupType**</span><span class="sxs-lookup"><span data-stu-id="f9cad-105">**ImGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9cad-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f9cad-106">Attributes and elements</span></span>

<span data-ttu-id="f9cad-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f9cad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9cad-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9cad-108">Attributes</span></span>

<span data-ttu-id="f9cad-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f9cad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9cad-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f9cad-110">Child elements</span></span>

<span data-ttu-id="f9cad-111">[DisplayName (非 Emptystringtype)](displayname-nonemptystringtype.md)  | [GroupType](grouptype.md)  | [ExchangeStoreId](exchangestoreid.md)  | [Membercorrelationkey](membercorrelationkey.md)  | [Extendedproperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)  | [Smtpaddress](smtpaddress.md)</span><span class="sxs-lookup"><span data-stu-id="f9cad-111">[DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupType](grouptype.md) | [ExchangeStoreId](exchangestoreid.md) | [MemberCorrelationKey](membercorrelationkey.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md) | [SmtpAddress](smtpaddress.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f9cad-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f9cad-112">Parent elements</span></span>

<span data-ttu-id="f9cad-113">[グループ (ArrayOfImGroupType)](groups-arrayofimgrouptype.md)  | [Adddeploy Grouptoimlistresponse](adddistributiongrouptoimlistresponse.md)  | [AddImGroupResponse](addimgroupresponse.md)</span><span class="sxs-lookup"><span data-stu-id="f9cad-113">[Groups (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md) | [AddImGroupResponse](addimgroupresponse.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f9cad-114">注釈</span><span class="sxs-lookup"><span data-stu-id="f9cad-114">Remarks</span></span>

<span data-ttu-id="f9cad-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f9cad-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f9cad-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f9cad-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9cad-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f9cad-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9cad-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="f9cad-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f9cad-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f9cad-119">Schema name</span></span>  <br/> |<span data-ttu-id="f9cad-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f9cad-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f9cad-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f9cad-121">Validation file</span></span>  <br/> |<span data-ttu-id="f9cad-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f9cad-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f9cad-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f9cad-123">Can be empty</span></span>  <br/> ||
   

