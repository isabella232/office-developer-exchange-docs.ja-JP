---
title: 迎える
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5a84c19e-57cd-448e-af4f-c8005fd5f2a2
description: 誕生日要素は、誕生日の配列、文字列として格納されたもの、および関連するペルソナのソース attributions の識別子を指定します。
ms.openlocfilehash: aa85febd84c32ae87e0822ce47fd99f445b6fe9e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462760"
---
# <a name="birthdays"></a><span data-ttu-id="4dbf5-103">迎える</span><span class="sxs-lookup"><span data-stu-id="4dbf5-103">Birthdays</span></span>

<span data-ttu-id="4dbf5-104">**誕生日**要素は、誕生日の配列、文字列として格納されたもの、および関連するペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="4dbf5-104">The **Birthdays** element specifies an array of birthdays, stored as strings, and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Birthdays>
   <StringAttributedValue/>
</Birthdays>
```

 <span data-ttu-id="4dbf5-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="4dbf5-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4dbf5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4dbf5-106">Attributes and elements</span></span>

<span data-ttu-id="4dbf5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4dbf5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4dbf5-108">属性</span><span class="sxs-lookup"><span data-stu-id="4dbf5-108">Attributes</span></span>

<span data-ttu-id="4dbf5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4dbf5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4dbf5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4dbf5-110">Child elements</span></span>

|<span data-ttu-id="4dbf5-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="4dbf5-111">**Element**</span></span>|<span data-ttu-id="4dbf5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4dbf5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4dbf5-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="4dbf5-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="4dbf5-114">Persona 要素に関連付けられている属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="4dbf5-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4dbf5-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4dbf5-115">Parent elements</span></span>

|<span data-ttu-id="4dbf5-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4dbf5-116">**Element**</span></span>|<span data-ttu-id="4dbf5-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4dbf5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4dbf5-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="4dbf5-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="4dbf5-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="4dbf5-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4dbf5-120">注釈</span><span class="sxs-lookup"><span data-stu-id="4dbf5-120">Remarks</span></span>

<span data-ttu-id="4dbf5-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4dbf5-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4dbf5-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4dbf5-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4dbf5-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4dbf5-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4dbf5-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="4dbf5-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4dbf5-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4dbf5-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4dbf5-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="4dbf5-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4dbf5-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4dbf5-127">Validation File</span></span>  <br/> |<span data-ttu-id="4dbf5-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="4dbf5-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4dbf5-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4dbf5-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4dbf5-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="4dbf5-130">See also</span></span>



- [<span data-ttu-id="4dbf5-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4dbf5-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

