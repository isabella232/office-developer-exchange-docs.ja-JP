---
title: AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cff8ef19-3e19-4107-9b35-c8a2b87a41bc
description: AddNewTelUriContactToGroup 要素は、AddNewTelUriContactToGroup の WSDL 操作の入力データを指定します。
ms.openlocfilehash: d99d557530397aa9edd2c23b595bdcb348783dd4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759292"
---
# <a name="addnewteluricontacttogroup"></a><span data-ttu-id="055f3-103">AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="055f3-103">AddNewTelUriContactToGroup</span></span>

<span data-ttu-id="055f3-104">**AddNewTelUriContactToGroup**要素は、 **AddNewTelUriContactToGroup**の WSDL 操作の入力データを指定します。</span><span class="sxs-lookup"><span data-stu-id="055f3-104">The **AddNewTelUriContactToGroup** element specifies the input data for the **AddNewTelUriContactToGroup** WSDL operation.</span></span> 
  
```XML
<AddNewTelUriContactToGroup>
   <TelUriAddress/>
   <ImContactSipUriAddress/>
   <ImTelephoneNumber/>
   <GroupId/>
</AddNewTelUriContactToGroup>
```

 <span data-ttu-id="055f3-105">**AddNewTelUriContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="055f3-105">**AddNewTelUriContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="055f3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="055f3-106">Attributes and elements</span></span>

<span data-ttu-id="055f3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="055f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="055f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="055f3-108">Attributes</span></span>

<span data-ttu-id="055f3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="055f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="055f3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="055f3-110">Child elements</span></span>

<span data-ttu-id="055f3-111">[TelUriAddress](teluriaddress.md) | [ImContactSipUriAddress](imcontactsipuriaddress.md) | [ImTelephoneNumber](imtelephonenumber.md) | [グループ Id](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="055f3-111">[TelUriAddress](teluriaddress.md) | [ImContactSipUriAddress](imcontactsipuriaddress.md) | [ImTelephoneNumber](imtelephonenumber.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="055f3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="055f3-112">Parent elements</span></span>

<span data-ttu-id="055f3-113">なし。</span><span class="sxs-lookup"><span data-stu-id="055f3-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="055f3-114">備考</span><span class="sxs-lookup"><span data-stu-id="055f3-114">Remarks</span></span>

<span data-ttu-id="055f3-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="055f3-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="055f3-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="055f3-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="055f3-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="055f3-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="055f3-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="055f3-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="055f3-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="055f3-119">Schema name</span></span>  <br/> |<span data-ttu-id="055f3-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="055f3-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="055f3-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="055f3-121">Validation file</span></span>  <br/> |<span data-ttu-id="055f3-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="055f3-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="055f3-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="055f3-123">Can be empty</span></span>  <br/> |<span data-ttu-id="055f3-124">False</span><span class="sxs-lookup"><span data-stu-id="055f3-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="055f3-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="055f3-125">See also</span></span>

- [<span data-ttu-id="055f3-126">AddNewTelUriContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="055f3-126">AddNewTelUriContactToGroup operation</span></span>](addnewteluricontacttogroup-operation.md)
- [<span data-ttu-id="055f3-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="055f3-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

