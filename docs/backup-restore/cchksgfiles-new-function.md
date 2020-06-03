---
title: CChkSGFiles.New 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: d18d3ef20890012a1d8c193ec87bdca10a1ed451
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455234"
---
# <a name="cchksgfilesnew-function"></a><span data-ttu-id="bc037-103">CChkSGFiles.New 関数</span><span class="sxs-lookup"><span data-stu-id="bc037-103">CChkSGFiles.New function</span></span>

<span data-ttu-id="bc037-104">**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="bc037-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="bc037-105">**CChkSGFiles** クラスの新しいインスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="bc037-105">Creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="bc037-106">この関数を呼び出してから、確認するストレージ グループとデータベースを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bc037-106">You must call this function before you can specify the storage group and databases to be checked.</span></span> 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a><span data-ttu-id="bc037-107">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bc037-107">Parameters</span></span>

<span data-ttu-id="bc037-108">なし。</span><span class="sxs-lookup"><span data-stu-id="bc037-108">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="bc037-109">Return value</span><span class="sxs-lookup"><span data-stu-id="bc037-109">Return value</span></span>

<span data-ttu-id="bc037-110">新しく作成されたオブジェクトへの参照 (ポインター)。</span><span class="sxs-lookup"><span data-stu-id="bc037-110">A reference (pointer) to the newly created object.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bc037-111">注釈</span><span class="sxs-lookup"><span data-stu-id="bc037-111">Remarks</span></span>

<span data-ttu-id="bc037-112">**New** 関数は、**CCheckSGFiles** オブジェクトを作成して、そのオブジェクトへの参照 (ポインター) を呼び出し元に返します。</span><span class="sxs-lookup"><span data-stu-id="bc037-112">The **New** function creates a **CCheckSGFiles** object and returns to the caller a reference (pointer) to that object.</span></span> <span data-ttu-id="bc037-113">この関数を最初に呼び出してから、**CCheckSGFiles** クラスのその他の関数を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="bc037-113">You must call this function before it calls any of the other functions in the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="bc037-114">マルチスレッド アプリケーションで CHKSGFILES を使用している場合は、そのアプリケーションのシングルスレッドの部分で **New** 関数を呼び出す必要があります。また、その関数は **CCheckSGFiles** オブジェクトごとに 1 回だけ呼び出すことができます。 </span><span class="sxs-lookup"><span data-stu-id="bc037-114">If you're using CHKSGFILES in a multithreaded application, you must call the **New** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="bc037-115">Requirements</span><span class="sxs-lookup"><span data-stu-id="bc037-115">Requirements</span></span>

<span data-ttu-id="bc037-116">Exchange 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bc037-116">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="bc037-117">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc037-117">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

