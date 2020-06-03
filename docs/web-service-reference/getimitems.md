---
title: GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 455e5709-6c06-49fd-bfb2-403fc912287c
description: GetImItems 要求要素は、指定されたインスタントメッセージンググループとインスタントメッセージングの連絡先ペルソナに関する情報を取得するための要求を定義します。
ms.openlocfilehash: e3973cbbf800ffe91472b9c733c4d4a927b91c9f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456452"
---
# <a name="getimitems"></a><span data-ttu-id="74840-103">GetImItems</span><span class="sxs-lookup"><span data-stu-id="74840-103">GetImItems</span></span>

<span data-ttu-id="74840-104">**Getimitems**要求要素は、指定されたインスタントメッセージンググループとインスタントメッセージングの連絡先ペルソナに関する情報を取得するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="74840-104">The **GetImItems** request element defines a request to get information about the specified instant messaging groups and instant messaging contact personas.</span></span> 
  
```XML
<GetImItems>
   <ContactIds/>
   <GroupIds/>
   <ExtendedProperties/>
</GetImItems>
```

 <span data-ttu-id="74840-105">**GetImItemsType**</span><span class="sxs-lookup"><span data-stu-id="74840-105">**GetImItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74840-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="74840-106">Attributes and elements</span></span>

<span data-ttu-id="74840-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="74840-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74840-108">属性</span><span class="sxs-lookup"><span data-stu-id="74840-108">Attributes</span></span>

<span data-ttu-id="74840-109">なし。</span><span class="sxs-lookup"><span data-stu-id="74840-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74840-110">子要素</span><span class="sxs-lookup"><span data-stu-id="74840-110">Child elements</span></span>

<span data-ttu-id="74840-111">[ContactIds](contactids.md)  | [Groupids](groupids.md)  | [Extendedproperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span><span class="sxs-lookup"><span data-stu-id="74840-111">[ContactIds](contactids.md) | [GroupIds](groupids.md) | [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="74840-112">親要素</span><span class="sxs-lookup"><span data-stu-id="74840-112">Parent elements</span></span>

<span data-ttu-id="74840-113">なし。</span><span class="sxs-lookup"><span data-stu-id="74840-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74840-114">注釈</span><span class="sxs-lookup"><span data-stu-id="74840-114">Remarks</span></span>

<span data-ttu-id="74840-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="74840-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="74840-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="74840-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74840-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="74840-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74840-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="74840-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74840-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="74840-119">Schema name</span></span>  <br/> |<span data-ttu-id="74840-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="74840-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74840-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="74840-121">Validation file</span></span>  <br/> |<span data-ttu-id="74840-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="74840-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74840-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="74840-123">Can be empty</span></span>  <br/> ||
   

