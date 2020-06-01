---
title: New-retentionpolicytag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: New-retentionpolicytag 要素は、メールボックスアイテムのアイテム保持ポリシーを指定します。
ms.openlocfilehash: 3ece841e14e6cf11ab15e4a4d8b83a778ae32e46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465178"
---
# <a name="retentionpolicytag"></a><span data-ttu-id="0a193-103">New-retentionpolicytag</span><span class="sxs-lookup"><span data-stu-id="0a193-103">RetentionPolicyTag</span></span>

<span data-ttu-id="0a193-104">**New-retentionpolicytag**要素は、メールボックスアイテムのアイテム保持ポリシーを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a193-104">The **RetentionPolicyTag** element specifies the retention policy for a mailbox item.</span></span> 
  
```XML
<RetentionPolicyTag>
   <DisplayName/>
   <RetentionId/>
   <RetentionPeriod/>
   <Type/>
   <RetentionAction/>
   <Description/>
   <IsVisible/>
   <OptedInto/>
   <IsArchive/>
</RetentionPolicyTag>
```

 <span data-ttu-id="0a193-105">**RetentionPolicyTagType**</span><span class="sxs-lookup"><span data-stu-id="0a193-105">**RetentionPolicyTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a193-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0a193-106">Attributes and elements</span></span>

<span data-ttu-id="0a193-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0a193-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a193-108">属性</span><span class="sxs-lookup"><span data-stu-id="0a193-108">Attributes</span></span>

<span data-ttu-id="0a193-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0a193-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a193-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0a193-110">Child elements</span></span>

<span data-ttu-id="0a193-111">[DisplayName (文字列)](displayname-string.md)  | [RetentionId](retentionid.md)  | [保存期間](retentionperiod.md)  | [Type (ElcFolderType)](type-elcfoldertype.md)  | [Retentionaction](retentionaction.md)  | [説明](description.md)  | [IsVisible](isvisible.md)  | [Optedinto](optedinto.md)  | [Isarchive](isarchive.md)</span><span class="sxs-lookup"><span data-stu-id="0a193-111">[DisplayName (string)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [Type (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [Description](description.md) | [IsVisible](isvisible.md) | [OptedInto](optedinto.md) | [IsArchive](isarchive.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0a193-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0a193-112">Parent elements</span></span>

[<span data-ttu-id="0a193-113">RetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="0a193-113">RetentionPolicyTags</span></span>](retentionpolicytags.md)
  
## <a name="remarks"></a><span data-ttu-id="0a193-114">注釈</span><span class="sxs-lookup"><span data-stu-id="0a193-114">Remarks</span></span>

<span data-ttu-id="0a193-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0a193-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0a193-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0a193-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a193-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0a193-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a193-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="0a193-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0a193-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0a193-119">Schema name</span></span>  <br/> |<span data-ttu-id="0a193-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0a193-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="0a193-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0a193-121">Validation file</span></span>  <br/> |<span data-ttu-id="0a193-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0a193-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0a193-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0a193-123">Can be empty</span></span>  <br/> ||
   

