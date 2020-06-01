---
title: CChkSGFiles.Delete 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: 38cb72b42727855f652de607bb2a02ecdeaae16e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44447051"
---
# <a name="cchksgfilesdelete-function"></a><span data-ttu-id="5dba0-103">CChkSGFiles.Delete 関数</span><span class="sxs-lookup"><span data-stu-id="5dba0-103">CChkSGFiles.Delete function</span></span>

<span data-ttu-id="5dba0-104">**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="5dba0-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="5dba0-105">**CChkSGFiles** クラスの既存のインスタンスを破棄します。</span><span class="sxs-lookup"><span data-stu-id="5dba0-105">Destroys an existing instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="5dba0-106">この関数は、アプリケーションが特定のオブジェクトの操作を完了した後で呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="5dba0-106">You must call this function after the application has finished working with the specified object.</span></span> 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a><span data-ttu-id="5dba0-107">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5dba0-107">Parameters</span></span>

### <a name="pcchecksgfiles"></a><span data-ttu-id="5dba0-108">pcchecksgfiles</span><span class="sxs-lookup"><span data-stu-id="5dba0-108">pcchecksgfiles</span></span> 
  
<span data-ttu-id="5dba0-109">入力パラメーター。</span><span class="sxs-lookup"><span data-stu-id="5dba0-109">Input parameter.</span></span> <span data-ttu-id="5dba0-110">既存の **CCheckSGFiles** オブジェクトへのポインターです。</span><span class="sxs-lookup"><span data-stu-id="5dba0-110">A pointer to an existing **CCheckSGFiles** object.</span></span> <span data-ttu-id="5dba0-111">オブジェクトに関連付けられていたメモリは解放されます。</span><span class="sxs-lookup"><span data-stu-id="5dba0-111">The memory associated with the object will then be freed.</span></span> 
    
## <a name="return-value"></a><span data-ttu-id="5dba0-112">Return value</span><span class="sxs-lookup"><span data-stu-id="5dba0-112">Return value</span></span>

<span data-ttu-id="5dba0-113">なし。</span><span class="sxs-lookup"><span data-stu-id="5dba0-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5dba0-114">注釈</span><span class="sxs-lookup"><span data-stu-id="5dba0-114">Remarks</span></span>

<span data-ttu-id="5dba0-115">**Delete** 関数は、**CCheckSGFiles** オブジェクトに関連付けられていたメモリを解放します。</span><span class="sxs-lookup"><span data-stu-id="5dba0-115">The **Delete** function frees the memory associated with the **CCheckSGFiles** object.</span></span> <span data-ttu-id="5dba0-116">**Delete**を呼び出した後は、 *pcchecksgfiles*パラメーターで渡されたポインターが無効になり、そのオブジェクトに対して他の操作を実行することはできません。</span><span class="sxs-lookup"><span data-stu-id="5dba0-116">After you call **Delete**, the pointer passed in the  *pcchecksgfiles*  parameter will be invalid and no other operations can be performed on that object.</span></span> 
  
<span data-ttu-id="5dba0-117">アプリケーションで **ErrCheckDbPages** 関数を使用する場合、そのアプリケーションではメモリ バッファーを手動で開放する必要があります。**Delete** 関数はメモリ バッファーを解放しません。</span><span class="sxs-lookup"><span data-stu-id="5dba0-117">If the application uses the **ErrCheckDbPages** function, the application must free the memory buffer manually; the **Delete** function will not free it.</span></span> 
  
<span data-ttu-id="5dba0-118">マルチスレッド アプリケーションで CHKSGFILES を使用している場合は、そのアプリケーションのシングルスレッドの部分で **Delete** 関数を呼び出す必要があります。また、その関数は **CCheckSGFiles** オブジェクトごとに 1 回だけ呼び出すことができます。 </span><span class="sxs-lookup"><span data-stu-id="5dba0-118">If you're using CHKSGFILES in a multithreaded application, you must call the **Delete** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="5dba0-119">Requirements</span><span class="sxs-lookup"><span data-stu-id="5dba0-119">Requirements</span></span>

<span data-ttu-id="5dba0-120">Exchange 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5dba0-120">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="5dba0-121">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="5dba0-121">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

