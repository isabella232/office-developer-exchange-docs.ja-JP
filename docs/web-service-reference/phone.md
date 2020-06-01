---
title: 電話番号
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9381d8e0-b705-49fd-a822-00fb485bdbab
description: Phone 要素は、連絡先エンティティの抽出から得られる1つの電話番号を指定します。
ms.openlocfilehash: 7b0047eda90f2e2bb94fd7d0b8d317715ac5d2c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459708"
---
# <a name="phone"></a><span data-ttu-id="47d2a-103">電話番号</span><span class="sxs-lookup"><span data-stu-id="47d2a-103">Phone</span></span>

<span data-ttu-id="47d2a-104">**Phone**要素は、連絡先エンティティの抽出から得られる1つの電話番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="47d2a-104">The **Phone** element specifies a single phone number that results from a contact entity extraction.</span></span> 
  
```XML
<Phone>
   <OriginalPhoneString/>
   <PhoneString/>
   <Type/>
</Phone>
```

 <span data-ttu-id="47d2a-105">**PhoneType**</span><span class="sxs-lookup"><span data-stu-id="47d2a-105">**PhoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47d2a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="47d2a-106">Attributes and elements</span></span>

<span data-ttu-id="47d2a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="47d2a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47d2a-108">属性</span><span class="sxs-lookup"><span data-stu-id="47d2a-108">Attributes</span></span>

<span data-ttu-id="47d2a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="47d2a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47d2a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="47d2a-110">Child elements</span></span>

<span data-ttu-id="47d2a-111">[Phonenumber.originalphonestring](originalphonestring.md)  | [電話テキスト](phonestring.md)  | [型 (string)](type-string.md)</span><span class="sxs-lookup"><span data-stu-id="47d2a-111">[OriginalPhoneString](originalphonestring.md) | [PhoneString](phonestring.md) | [Type (string)](type-string.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="47d2a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="47d2a-112">Parent elements</span></span>

[<span data-ttu-id="47d2a-113">PhoneNumbers (ArrayOfPhonesType)</span><span class="sxs-lookup"><span data-stu-id="47d2a-113">PhoneNumbers (ArrayOfPhonesType)</span></span>](phonenumbers-arrayofphonestype.md)
  
## <a name="remarks"></a><span data-ttu-id="47d2a-114">注釈</span><span class="sxs-lookup"><span data-stu-id="47d2a-114">Remarks</span></span>

<span data-ttu-id="47d2a-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="47d2a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="47d2a-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="47d2a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47d2a-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="47d2a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47d2a-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="47d2a-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="47d2a-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="47d2a-119">Schema name</span></span>  <br/> |<span data-ttu-id="47d2a-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="47d2a-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="47d2a-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="47d2a-121">Validation file</span></span>  <br/> |<span data-ttu-id="47d2a-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="47d2a-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="47d2a-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="47d2a-123">Can be empty</span></span>  <br/> ||
   

