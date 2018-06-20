---
title: CChkSGFiles.CMaxDbPerSG 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CMaxDbPerSG
api_type:
- dllExport
ms.assetid: 5871988b-a5d7-42cc-9b83-8fededb5072f
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: bf09074bab6dee13e97e8a59a22ae1b19522a5e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759824"
---
# <a name="cchksgfilescmaxdbpersg-function"></a><span data-ttu-id="a831a-103">CChkSGFiles.CMaxDbPerSG 関数</span><span class="sxs-lookup"><span data-stu-id="a831a-103">CChkSGFiles.CMaxDbPerSG function</span></span>

<span data-ttu-id="a831a-104">**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="a831a-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="a831a-105">1 つの Exchange サーバー ストレージ グループに許容されるデータベースの最大数を返します。</span><span class="sxs-lookup"><span data-stu-id="a831a-105">Returns the maximum number of databases allowed in a single Exchange server storage group.</span></span>
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a><span data-ttu-id="a831a-106">Parameters</span><span class="sxs-lookup"><span data-stu-id="a831a-106">Parameters</span></span>

<span data-ttu-id="a831a-107">なし。</span><span class="sxs-lookup"><span data-stu-id="a831a-107">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="a831a-108">Return value</span><span class="sxs-lookup"><span data-stu-id="a831a-108">Return value</span></span>

<span data-ttu-id="a831a-109">指定された Exchange サーバーでは、ストレージ グループあたりのデータベースの最大数です。</span><span class="sxs-lookup"><span data-stu-id="a831a-109">The maximum number of databases that the specified Exchange server allows per storage group.</span></span> <span data-ttu-id="a831a-110">ストレージ ・ グループは Exchange 2013 の一部ではないため、この関数は 1 を返します。</span><span class="sxs-lookup"><span data-stu-id="a831a-110">Because storage groups are not part of Exchange 2013, this function returns 1.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a831a-111">備考</span><span class="sxs-lookup"><span data-stu-id="a831a-111">Remarks</span></span>

<span data-ttu-id="a831a-112">**CMaxDbPerSG**関数によって返される値もチェックを使用してデータベースの最大数を表すように、1 つのストレージ ・ グループに (データベースとトランザクション ログ ファイル) を検証する**CCheckSGFiles**オブジェクトを使用することができます、**CCheckSGFiles**クラスのインスタンスです。</span><span class="sxs-lookup"><span data-stu-id="a831a-112">You can use the **CCheckSGFiles** object to validate databases (and transaction log files) in only one storage group, so the value returned by the **CMaxDbPerSG** function also represents the maximum number of databases that you can check by using an instance of the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="a831a-113">既定では、Exchange Server 2003 と Exchange Server 2007 を許可する最大のストレージ グループあたり 5 データベースに注意してください。</span><span class="sxs-lookup"><span data-stu-id="a831a-113">Note that by default, Exchange Server 2003 and Exchange Server 2007 allow a maximum of five databases per storage group.</span></span>
  
## <a name="requirements"></a><span data-ttu-id="a831a-114">必要条件</span><span class="sxs-lookup"><span data-stu-id="a831a-114">Requirements</span></span>

<span data-ttu-id="a831a-115">Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="a831a-115">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="a831a-116">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="a831a-116">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

