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
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: b40f8b1a95477715b29defb4addabfb333e92d04
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758856"
---
# <a name="cchksgfilesnew-function"></a><span data-ttu-id="4a573-103">CChkSGFiles.New 関数</span><span class="sxs-lookup"><span data-stu-id="4a573-103">CChkSGFiles.New function</span></span>

<span data-ttu-id="4a573-104">**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="4a573-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="4a573-105">**CChkSGFiles**クラスの新しいインスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="4a573-105">Creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="4a573-106">チェックするには、ストレージ グループおよびデータベースを指定する前に、この関数を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a573-106">You must call this function before you can specify the storage group and databases to be checked.</span></span> 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a><span data-ttu-id="4a573-107">Parameters</span><span class="sxs-lookup"><span data-stu-id="4a573-107">Parameters</span></span>

<span data-ttu-id="4a573-108">なし。</span><span class="sxs-lookup"><span data-stu-id="4a573-108">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="4a573-109">Return value</span><span class="sxs-lookup"><span data-stu-id="4a573-109">Return value</span></span>

<span data-ttu-id="4a573-110">新しく作成されたオブジェクトへの参照 (ポインター)。</span><span class="sxs-lookup"><span data-stu-id="4a573-110">A reference (pointer) to the newly created object.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4a573-111">備考</span><span class="sxs-lookup"><span data-stu-id="4a573-111">Remarks</span></span>

<span data-ttu-id="4a573-112">**新規**の関数は、 **CCheckSGFiles**オブジェクトを作成し、そのオブジェクトへの参照 (ポインター) を呼び出し元に返します。</span><span class="sxs-lookup"><span data-stu-id="4a573-112">The **New** function creates a **CCheckSGFiles** object and returns to the caller a reference (pointer) to that object.</span></span> <span data-ttu-id="4a573-113">**CCheckSGFiles**クラスのすべての他の関数を呼び出す前にこの関数を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a573-113">You must call this function before it calls any of the other functions in the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="4a573-114">マルチ スレッド アプリケーションで CHKSGFILES を使用する場合、シングル スレッド アプリケーションの部分で、**新規**の関数を呼び出す必要があり、 **CCheckSGFiles**オブジェクトごとに 1 回のみ呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="4a573-114">If you're using CHKSGFILES in a multithreaded application, you must call the **New** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="4a573-115">必要条件</span><span class="sxs-lookup"><span data-stu-id="4a573-115">Requirements</span></span>

<span data-ttu-id="4a573-116">Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="4a573-116">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="4a573-117">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a573-117">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

