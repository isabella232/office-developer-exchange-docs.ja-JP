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
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: 5c41007a797e5a256692b2c4bdcb3cfae82c12ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758862"
---
# <a name="cchksgfilesdelete-function"></a><span data-ttu-id="df6f3-103">CChkSGFiles.Delete 関数</span><span class="sxs-lookup"><span data-stu-id="df6f3-103">CChkSGFiles.Delete function</span></span>

<span data-ttu-id="df6f3-104">**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="df6f3-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="df6f3-105">**CChkSGFiles**クラスの既存のインスタンスを破棄します。</span><span class="sxs-lookup"><span data-stu-id="df6f3-105">Destroys an existing instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="df6f3-106">アプリケーションが指定したオブジェクトの操作を完了した後は、この関数を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="df6f3-106">You must call this function after the application has finished working with the specified object.</span></span> 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a><span data-ttu-id="df6f3-107">Parameters</span><span class="sxs-lookup"><span data-stu-id="df6f3-107">Parameters</span></span>

### <a name="pcchecksgfiles"></a><span data-ttu-id="df6f3-108">pcchecksgfiles</span><span class="sxs-lookup"><span data-stu-id="df6f3-108">pcchecksgfiles</span></span> 
  
<span data-ttu-id="df6f3-109">パラメーターを入力します。</span><span class="sxs-lookup"><span data-stu-id="df6f3-109">Input parameter.</span></span> <span data-ttu-id="df6f3-110">既存の**CCheckSGFiles**オブジェクトへのポインター。</span><span class="sxs-lookup"><span data-stu-id="df6f3-110">A pointer to an existing **CCheckSGFiles** object.</span></span> <span data-ttu-id="df6f3-111">オブジェクトに関連付けられているメモリを解放し、されます。</span><span class="sxs-lookup"><span data-stu-id="df6f3-111">The memory associated with the object will then be freed.</span></span> 
    
## <a name="return-value"></a><span data-ttu-id="df6f3-112">Return value</span><span class="sxs-lookup"><span data-stu-id="df6f3-112">Return value</span></span>

<span data-ttu-id="df6f3-113">なし。</span><span class="sxs-lookup"><span data-stu-id="df6f3-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="df6f3-114">備考</span><span class="sxs-lookup"><span data-stu-id="df6f3-114">Remarks</span></span>

<span data-ttu-id="df6f3-115">**削除**関数は、 **CCheckSGFiles**オブジェクトに関連付けられているメモリを解放します。</span><span class="sxs-lookup"><span data-stu-id="df6f3-115">The **Delete** function frees the memory associated with the **CCheckSGFiles** object.</span></span> <span data-ttu-id="df6f3-116">**削除**を呼び出すと、 *pcchecksgfiles*パラメーターに渡されたポインターが無効になりそのオブジェクトの他の操作を実行されません。</span><span class="sxs-lookup"><span data-stu-id="df6f3-116">After you call **Delete**, the pointer passed in the  *pcchecksgfiles*  parameter will be invalid and no other operations can be performed on that object.</span></span> 
  
<span data-ttu-id="df6f3-117">アプリケーションがメモリ バッファーを手動で解放する必要がありますアプリケーションでは、 **ErrCheckDbPages**関数を使用する場合**削除**関数では、解放はしません。</span><span class="sxs-lookup"><span data-stu-id="df6f3-117">If the application uses the **ErrCheckDbPages** function, the application must free the memory buffer manually; the **Delete** function will not free it.</span></span> 
  
<span data-ttu-id="df6f3-118">マルチ スレッド アプリケーションで CHKSGFILES を使用する場合、シングル スレッド アプリケーションの部分で**削除**関数を呼び出す必要があり、 **CCheckSGFiles**オブジェクトごとに 1 回のみ呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="df6f3-118">If you're using CHKSGFILES in a multithreaded application, you must call the **Delete** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="df6f3-119">必要条件</span><span class="sxs-lookup"><span data-stu-id="df6f3-119">Requirements</span></span>

<span data-ttu-id="df6f3-120">Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="df6f3-120">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="df6f3-121">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="df6f3-121">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

