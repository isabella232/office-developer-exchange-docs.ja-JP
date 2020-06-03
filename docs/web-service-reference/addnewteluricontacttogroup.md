---
title: AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cff8ef19-3e19-4107-9b35-c8a2b87a41bc
description: AddNewTelUriContactToGroup 要素は、AddNewTelUriContactToGroup WSDL 操作の入力データを指定します。
ms.openlocfilehash: 151c5b1dab7a3ffc9630fb4e4192b90bd1d4ae38
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464932"
---
# <a name="addnewteluricontacttogroup"></a><span data-ttu-id="dc986-103">AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="dc986-103">AddNewTelUriContactToGroup</span></span>

<span data-ttu-id="dc986-104">**AddNewTelUriContactToGroup**要素は、 **AddNewTelUriContactToGroup** WSDL 操作の入力データを指定します。</span><span class="sxs-lookup"><span data-stu-id="dc986-104">The **AddNewTelUriContactToGroup** element specifies the input data for the **AddNewTelUriContactToGroup** WSDL operation.</span></span> 
  
```XML
<AddNewTelUriContactToGroup>
   <TelUriAddress/>
   <ImContactSipUriAddress/>
   <ImTelephoneNumber/>
   <GroupId/>
</AddNewTelUriContactToGroup>
```

 <span data-ttu-id="dc986-105">**AddNewTelUriContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="dc986-105">**AddNewTelUriContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc986-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dc986-106">Attributes and elements</span></span>

<span data-ttu-id="dc986-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dc986-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc986-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc986-108">Attributes</span></span>

<span data-ttu-id="dc986-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dc986-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc986-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dc986-110">Child elements</span></span>

<span data-ttu-id="dc986-111">[Teluriaddress](teluriaddress.md)  | [Imcontactsi紫 Iaddress](imcontactsipuriaddress.md)  | [ImTelephoneNumber](imtelephonenumber.md)  | [GroupId](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="dc986-111">[TelUriAddress](teluriaddress.md) | [ImContactSipUriAddress](imcontactsipuriaddress.md) | [ImTelephoneNumber](imtelephonenumber.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dc986-112">親要素</span><span class="sxs-lookup"><span data-stu-id="dc986-112">Parent elements</span></span>

<span data-ttu-id="dc986-113">なし。</span><span class="sxs-lookup"><span data-stu-id="dc986-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dc986-114">注釈</span><span class="sxs-lookup"><span data-stu-id="dc986-114">Remarks</span></span>

<span data-ttu-id="dc986-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="dc986-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dc986-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dc986-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc986-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dc986-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc986-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="dc986-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dc986-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dc986-119">Schema name</span></span>  <br/> |<span data-ttu-id="dc986-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="dc986-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dc986-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dc986-121">Validation file</span></span>  <br/> |<span data-ttu-id="dc986-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="dc986-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dc986-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="dc986-123">Can be empty</span></span>  <br/> |<span data-ttu-id="dc986-124">正しくない</span><span class="sxs-lookup"><span data-stu-id="dc986-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc986-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="dc986-125">See also</span></span>

- [<span data-ttu-id="dc986-126">AddNewTelUriContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="dc986-126">AddNewTelUriContactToGroup operation</span></span>](addnewteluricontacttogroup-operation.md)
- [<span data-ttu-id="dc986-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="dc986-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

