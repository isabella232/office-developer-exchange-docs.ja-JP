---
title: SearchPreviewItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 59b0b2db-a0ae-4162-a2cb-5f37f42fe872
description: SearchPreviewItem 要素は、検索の検索項目のプレビューを指定します。
ms.openlocfilehash: 46b9d6049f856ce6e93b9e49e07516ec4b52d932
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833308"
---
# <a name="searchpreviewitem"></a><span data-ttu-id="46cfb-103">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="46cfb-103">SearchPreviewItem</span></span>

<span data-ttu-id="46cfb-104">**SearchPreviewItem**要素は、検索の検索項目のプレビューを指定します。</span><span class="sxs-lookup"><span data-stu-id="46cfb-104">The **SearchPreviewItem** element specifies the item preview for a discovery search.</span></span> 
  
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

 <span data-ttu-id="46cfb-105">**SearchPreviewItemType**</span><span class="sxs-lookup"><span data-stu-id="46cfb-105">**SearchPreviewItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46cfb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="46cfb-106">Attributes and elements</span></span>

<span data-ttu-id="46cfb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="46cfb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46cfb-108">属性</span><span class="sxs-lookup"><span data-stu-id="46cfb-108">Attributes</span></span>

<span data-ttu-id="46cfb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="46cfb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46cfb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="46cfb-110">Child elements</span></span>

<span data-ttu-id="46cfb-111">[ID (ItemIdType)](id-itemidtype.md) | [メールボックス (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [ParentId](parentid.md) | [ItemClass](itemclass.md) | [UniqueHash](uniquehash.md) | [SortValue](sortvalue.md) | [OwaLink](owalink.md)  |  [送信者 (文字列)](sender-string.md) | [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md) | [CcRecipients](ccrecipients.md) | [BccRecipients](bccrecipients.md) | [CreatedTime](createdtime.md) | [ReceivedTime](receivedtime.md)  | [SentTime](senttime.md) | [件名](subject.md) | [サイズ (長)](size-long.md) | [プレビュー](preview-ex15websvcsotherref.md) | [の重要性](importance.md) | [読み取り](read.md) | [添付ファイルあり](hasattachment.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span><span class="sxs-lookup"><span data-stu-id="46cfb-111">[ID (ItemIdType)](id-itemidtype.md) | [Mailbox (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [ParentId](parentid.md) | [ItemClass](itemclass.md) | [UniqueHash](uniquehash.md) | [SortValue](sortvalue.md) | [OwaLink](owalink.md) | [Sender (string)](sender-string.md) | [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md) | [CcRecipients](ccrecipients.md) | [BccRecipients](bccrecipients.md) | [CreatedTime](createdtime.md) | [ReceivedTime](receivedtime.md) | [SentTime](senttime.md) | [Subject](subject.md) | [Size (long)](size-long.md) | [Preview](preview-ex15websvcsotherref.md) | [Importance](importance.md) | [Read](read.md) | [HasAttachment](hasattachment.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="46cfb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="46cfb-112">Parent elements</span></span>

[<span data-ttu-id="46cfb-113">アイテム (ArrayOfSearchPreviewItemsType)</span><span class="sxs-lookup"><span data-stu-id="46cfb-113">Items (ArrayOfSearchPreviewItemsType)</span></span>](items-arrayofsearchpreviewitemstype.md)
  
## <a name="remarks"></a><span data-ttu-id="46cfb-114">備考</span><span class="sxs-lookup"><span data-stu-id="46cfb-114">Remarks</span></span>

<span data-ttu-id="46cfb-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="46cfb-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="46cfb-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="46cfb-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46cfb-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="46cfb-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46cfb-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="46cfb-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46cfb-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="46cfb-119">Schema name</span></span>  <br/> |<span data-ttu-id="46cfb-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="46cfb-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="46cfb-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="46cfb-121">Validation file</span></span>  <br/> |<span data-ttu-id="46cfb-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="46cfb-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46cfb-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="46cfb-123">Can be empty</span></span>  <br/> ||
   

