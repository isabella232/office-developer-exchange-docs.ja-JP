---
title: アプリ
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92b776b5-fec6-4443-a606-51ccb06f7afd
description: App 要素には、メールボックスにインストールされているメールアプリの XML マニフェストファイルに関する情報が含まれています。
ms.openlocfilehash: b5870164b059d2e50930ee33c09cbd030501f171
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460359"
---
# <a name="app"></a><span data-ttu-id="ebb1f-103">アプリ</span><span class="sxs-lookup"><span data-stu-id="ebb1f-103">App</span></span>

<span data-ttu-id="ebb1f-104">**App**要素には、メールボックスにインストールされているメールアプリの XML マニフェストファイルに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ebb1f-104">The **App** element contains information about an XML manifest file for a mail app that is installed in a mailbox.</span></span> 
  
```XML
<App>
    <Metadata/>
    <Manifest/>
</App>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="ebb1f-105">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ebb1f-105">Attributes and elements</span></span>

<span data-ttu-id="ebb1f-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ebb1f-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ebb1f-107">属性</span><span class="sxs-lookup"><span data-stu-id="ebb1f-107">Attributes</span></span>

<span data-ttu-id="ebb1f-108">なし。</span><span class="sxs-lookup"><span data-stu-id="ebb1f-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ebb1f-109">子要素</span><span class="sxs-lookup"><span data-stu-id="ebb1f-109">Child elements</span></span>

<span data-ttu-id="ebb1f-110">[メタデータ](metadata-ex15websvcsotherref.md)  | [マニフェスト](manifest.md)</span><span class="sxs-lookup"><span data-stu-id="ebb1f-110">[Metadata](metadata-ex15websvcsotherref.md) | [Manifest](manifest.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ebb1f-111">親要素</span><span class="sxs-lookup"><span data-stu-id="ebb1f-111">Parent elements</span></span>

[<span data-ttu-id="ebb1f-112">アプリ</span><span class="sxs-lookup"><span data-stu-id="ebb1f-112">Apps</span></span>](apps.md)
  
## <a name="remarks"></a><span data-ttu-id="ebb1f-113">注釈</span><span class="sxs-lookup"><span data-stu-id="ebb1f-113">Remarks</span></span>

<span data-ttu-id="ebb1f-114">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ebb1f-114">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="ebb1f-115">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ebb1f-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ebb1f-116">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ebb1f-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ebb1f-117">Namespace</span><span class="sxs-lookup"><span data-stu-id="ebb1f-117">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ebb1f-118">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ebb1f-118">Schema Name</span></span>  <br/> |<span data-ttu-id="ebb1f-119">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ebb1f-119">Types schema</span></span>  <br/> |
|<span data-ttu-id="ebb1f-120">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ebb1f-120">Validation File</span></span>  <br/> |<span data-ttu-id="ebb1f-121">該当なし</span><span class="sxs-lookup"><span data-stu-id="ebb1f-121">Not applicable</span></span>  <br/> |
|<span data-ttu-id="ebb1f-122">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ebb1f-122">Can be Empty</span></span>  <br/> |<span data-ttu-id="ebb1f-123">正しくない</span><span class="sxs-lookup"><span data-stu-id="ebb1f-123">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ebb1f-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="ebb1f-124">See also</span></span>

- [<span data-ttu-id="ebb1f-125">アプリ</span><span class="sxs-lookup"><span data-stu-id="ebb1f-125">Apps</span></span>](apps.md)
- [<span data-ttu-id="ebb1f-126">メタデータ</span><span class="sxs-lookup"><span data-stu-id="ebb1f-126">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="ebb1f-127">マニフェスト</span><span class="sxs-lookup"><span data-stu-id="ebb1f-127">Manifest</span></span>](manifest.md)
- [<span data-ttu-id="ebb1f-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ebb1f-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

