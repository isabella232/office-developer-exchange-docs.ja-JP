---
title: アプリ
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92b776b5-fec6-4443-a606-51ccb06f7afd
description: アプリケーション要素には、メールボックスにインストールされているメール アプリの XML マニフェスト ファイルに関する情報が含まれています。
ms.openlocfilehash: c63bbbf6eb3bf718b2cf81e67d9ec978b3bc5f8d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759330"
---
# <a name="app"></a><span data-ttu-id="23662-103">アプリ</span><span class="sxs-lookup"><span data-stu-id="23662-103">App</span></span>

<span data-ttu-id="23662-104">**アプリケーション**要素には、メールボックスにインストールされているメール アプリの XML マニフェスト ファイルに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="23662-104">The **App** element contains information about an XML manifest file for a mail app that is installed in a mailbox.</span></span> 
  
```XML
<App>
    <Metadata/>
    <Manifest/>
</App>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="23662-105">属性および要素</span><span class="sxs-lookup"><span data-stu-id="23662-105">Attributes and elements</span></span>

<span data-ttu-id="23662-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="23662-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23662-107">属性</span><span class="sxs-lookup"><span data-stu-id="23662-107">Attributes</span></span>

<span data-ttu-id="23662-108">なし。</span><span class="sxs-lookup"><span data-stu-id="23662-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23662-109">子要素</span><span class="sxs-lookup"><span data-stu-id="23662-109">Child elements</span></span>

<span data-ttu-id="23662-110">[メタデータ](metadata-ex15websvcsotherref.md) | [マニフェスト](manifest.md)</span><span class="sxs-lookup"><span data-stu-id="23662-110">[Metadata](metadata-ex15websvcsotherref.md) | [Manifest](manifest.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="23662-111">親要素</span><span class="sxs-lookup"><span data-stu-id="23662-111">Parent elements</span></span>

[<span data-ttu-id="23662-112">アプリ</span><span class="sxs-lookup"><span data-stu-id="23662-112">Apps</span></span>](apps.md)
  
## <a name="remarks"></a><span data-ttu-id="23662-113">備考</span><span class="sxs-lookup"><span data-stu-id="23662-113">Remarks</span></span>

<span data-ttu-id="23662-114">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="23662-114">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="23662-115">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="23662-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23662-116">要素情報</span><span class="sxs-lookup"><span data-stu-id="23662-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23662-117">名前空間</span><span class="sxs-lookup"><span data-stu-id="23662-117">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="23662-118">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="23662-118">Schema Name</span></span>  <br/> |<span data-ttu-id="23662-119">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="23662-119">Types schema</span></span>  <br/> |
|<span data-ttu-id="23662-120">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="23662-120">Validation File</span></span>  <br/> |<span data-ttu-id="23662-121">該当しない</span><span class="sxs-lookup"><span data-stu-id="23662-121">Not applicable</span></span>  <br/> |
|<span data-ttu-id="23662-122">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="23662-122">Can be Empty</span></span>  <br/> |<span data-ttu-id="23662-123">False</span><span class="sxs-lookup"><span data-stu-id="23662-123">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="23662-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="23662-124">See also</span></span>

- [<span data-ttu-id="23662-125">アプリ</span><span class="sxs-lookup"><span data-stu-id="23662-125">Apps</span></span>](apps.md)
- [<span data-ttu-id="23662-126">メタデータ</span><span class="sxs-lookup"><span data-stu-id="23662-126">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="23662-127">Manifest</span><span class="sxs-lookup"><span data-stu-id="23662-127">Manifest</span></span>](manifest.md)
- [<span data-ttu-id="23662-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="23662-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

