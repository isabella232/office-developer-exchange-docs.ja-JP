---
title: Searchプレビューアイテム
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 59b0b2db-a0ae-4162-a2cb-5f37f42fe872
description: Searchpreview Item 要素は、探索検索のアイテムプレビューを指定します。
ms.openlocfilehash: ab48353b0ffaf4bc3b9409f1a620d145bffc7a13
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466935"
---
# <a name="searchpreviewitem"></a><span data-ttu-id="e9bba-103">Searchプレビューアイテム</span><span class="sxs-lookup"><span data-stu-id="e9bba-103">SearchPreviewItem</span></span>

<span data-ttu-id="e9bba-104">**Searchpreview item**要素は、探索検索のアイテムプレビューを指定します。</span><span class="sxs-lookup"><span data-stu-id="e9bba-104">The **SearchPreviewItem** element specifies the item preview for a discovery search.</span></span> 
  
```XML
<SearchPreviewItem>
   <Id/>
   <Mailbox/>
   <ParentId/>
   <ItemClass/>
   <UniqueHash/>
   <SortValue/>
   <OwaLink/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <CreatedTime/>
   <ReceivedTime/>
   <SentTime/>
   <Subject/>
   <Size/>
   <Preview/>
   <Importance/>
   <Read/>
   <HasAttachment/>
   <ExtendedProperties/>
</SearchPreviewItem>
```

 <span data-ttu-id="e9bba-105">**Searchプレビュー Itemtype**</span><span class="sxs-lookup"><span data-stu-id="e9bba-105">**SearchPreviewItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9bba-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e9bba-106">Attributes and elements</span></span>

<span data-ttu-id="e9bba-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9bba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9bba-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9bba-108">Attributes</span></span>

<span data-ttu-id="e9bba-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e9bba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9bba-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e9bba-110">Child elements</span></span>

<span data-ttu-id="e9bba-111">[ID (ItemIdType)](id-itemidtype.md)  | [メールボックス (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md)  | [ParentId](parentid.md)  | [Itemclass](itemclass.md)  | [UniqueHash](uniquehash.md)  | [Sortvalue](sortvalue.md)  | [Owalink](owalink.md)  | [Sender (文字列)](sender-string.md)  | [Torの pipi(ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md)  | [Ccrecipients](ccrecipients.md)  |  イベント[Bccrecipients](bccrecipients.md)  |  イベント[ランタイム](createdtime.md)  | [ReceivedTime](receivedtime.md)  | [時間](senttime.md)  | [件名](subject.md)  | [サイズ (長い)](size-long.md)  | [プレビュー](preview-ex15websvcsotherref.md)  | [重要度](importance.md)  | [読み取り](read.md)  | [Hasattachment](hasattachment.md)  | [Extendedproperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span><span class="sxs-lookup"><span data-stu-id="e9bba-111">[ID (ItemIdType)](id-itemidtype.md) | [Mailbox (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [ParentId](parentid.md) | [ItemClass](itemclass.md) | [UniqueHash](uniquehash.md) | [SortValue](sortvalue.md) | [OwaLink](owalink.md) | [Sender (string)](sender-string.md) | [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md) | [CcRecipients](ccrecipients.md) | [BccRecipients](bccrecipients.md) | [CreatedTime](createdtime.md) | [ReceivedTime](receivedtime.md) | [SentTime](senttime.md) | [Subject](subject.md) | [Size (long)](size-long.md) | [Preview](preview-ex15websvcsotherref.md) | [Importance](importance.md) | [Read](read.md) | [HasAttachment](hasattachment.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e9bba-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e9bba-112">Parent elements</span></span>

[<span data-ttu-id="e9bba-113">アイテム (Arrayofsearchプレビュー Itemstype)</span><span class="sxs-lookup"><span data-stu-id="e9bba-113">Items (ArrayOfSearchPreviewItemsType)</span></span>](items-arrayofsearchpreviewitemstype.md)
  
## <a name="remarks"></a><span data-ttu-id="e9bba-114">注釈</span><span class="sxs-lookup"><span data-stu-id="e9bba-114">Remarks</span></span>

<span data-ttu-id="e9bba-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e9bba-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e9bba-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e9bba-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9bba-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e9bba-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9bba-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9bba-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9bba-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9bba-119">Schema name</span></span>  <br/> |<span data-ttu-id="e9bba-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e9bba-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9bba-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9bba-121">Validation file</span></span>  <br/> |<span data-ttu-id="e9bba-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e9bba-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9bba-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e9bba-123">Can be empty</span></span>  <br/> ||
   

