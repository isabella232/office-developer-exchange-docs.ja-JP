---
title: RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a62b0640-9800-45a6-a297-2105ff36881e
description: RemoveImContactFromGroup 要素は、インスタントメッセージンググループからインスタントメッセージングの連絡先を削除する要求を定義します。
ms.openlocfilehash: 379994ad5832b05e9f7da61d752f7660a6eec5ad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466963"
---
# <a name="removeimcontactfromgroup"></a><span data-ttu-id="ad6ef-103">RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="ad6ef-103">RemoveImContactFromGroup</span></span>

<span data-ttu-id="ad6ef-104">**Removeimcontactfromgroup**要素は、インスタントメッセージンググループからインスタントメッセージングの連絡先を削除する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="ad6ef-104">The **RemoveImContactFromGroup** element defines a request to remove an instant messaging contact from an instant messaging group.</span></span> 
  
```XML
<RemoveImContactFromGroup>
   <ContactId/>
   <GroupId/>
</RemoveImContactFromGroup>
```

 <span data-ttu-id="ad6ef-105">**RemoveImContactFromGroupType**</span><span class="sxs-lookup"><span data-stu-id="ad6ef-105">**RemoveImContactFromGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad6ef-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ad6ef-106">Attributes and elements</span></span>

<span data-ttu-id="ad6ef-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ad6ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad6ef-108">属性</span><span class="sxs-lookup"><span data-stu-id="ad6ef-108">Attributes</span></span>

<span data-ttu-id="ad6ef-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ad6ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad6ef-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ad6ef-110">Child elements</span></span>

<span data-ttu-id="ad6ef-111">[ContactId](contactid.md)  | [GroupId](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="ad6ef-111">[ContactId](contactid.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ad6ef-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ad6ef-112">Parent elements</span></span>

<span data-ttu-id="ad6ef-113">なし。</span><span class="sxs-lookup"><span data-stu-id="ad6ef-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ad6ef-114">注釈</span><span class="sxs-lookup"><span data-stu-id="ad6ef-114">Remarks</span></span>

<span data-ttu-id="ad6ef-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ad6ef-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ad6ef-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ad6ef-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad6ef-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ad6ef-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad6ef-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="ad6ef-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ad6ef-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ad6ef-119">Schema name</span></span>  <br/> |<span data-ttu-id="ad6ef-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="ad6ef-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ad6ef-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ad6ef-121">Validation file</span></span>  <br/> |<span data-ttu-id="ad6ef-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ad6ef-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ad6ef-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ad6ef-123">Can be empty</span></span>  <br/> ||
   

