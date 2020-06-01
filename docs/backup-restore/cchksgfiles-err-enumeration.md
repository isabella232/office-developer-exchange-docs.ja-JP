---
title: CChkSGFiles.ERR 列挙型
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ERR
api_type:
- dllExport
ms.assetid: f0efe195-91c3-4f3a-8c7d-e5dba336465a
description: '最終更新日: 2015 年 3 月 9 日'
ms.openlocfilehash: dbc76601a808f79ce3ed5b5dc9fbe4cf92efb015
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455255"
---
# <a name="cchksgfileserr-enumeration"></a><span data-ttu-id="b640a-103">CChkSGFiles.ERR 列挙型</span><span class="sxs-lookup"><span data-stu-id="b640a-103">CChkSGFiles.ERR enumeration</span></span> 
  
<span data-ttu-id="b640a-104">**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="b640a-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="b640a-105">呼び出された関数の結果を示します。</span><span class="sxs-lookup"><span data-stu-id="b640a-105">Indicates the results of the called function.</span></span> <span data-ttu-id="b640a-106">この列挙型は、**CCheckSGFiles** クラスの多数の関数によって返されます。</span><span class="sxs-lookup"><span data-stu-id="b640a-106">This enumeration is returned by many functions of the **CCheckSGFiles** class.</span></span> 
  
```cs
Enum ERR  
{
        errSuccess = 0,
        errTaskDropped = -106,
        errRequiredLogFilesMissing = -543,
        errInvalidParameter = -1003,
        errOutOfMemory = -1011,
        errReadVerifyFailure = -1018,
        errTooManyActiveUsers = -1059,
        errDatabaseCorrupted = -1206
}

```

## <a name="values"></a><span data-ttu-id="b640a-107">値</span><span class="sxs-lookup"><span data-stu-id="b640a-107">Values</span></span>

|<span data-ttu-id="b640a-108">**メンバー名**</span><span class="sxs-lookup"><span data-stu-id="b640a-108">**Member name**</span></span>|<span data-ttu-id="b640a-109">**値**</span><span class="sxs-lookup"><span data-stu-id="b640a-109">**Value**</span></span>|<span data-ttu-id="b640a-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="b640a-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b640a-111">errSuccess</span><span class="sxs-lookup"><span data-stu-id="b640a-111">errSuccess</span></span>  <br/> |<span data-ttu-id="b640a-112">.0</span><span class="sxs-lookup"><span data-stu-id="b640a-112">0</span></span>  <br/> |<span data-ttu-id="b640a-113">関数はエラーなしで正常に終了しました。</span><span class="sxs-lookup"><span data-stu-id="b640a-113">The function completed without any errors.</span></span>  <br/> |
|<span data-ttu-id="b640a-114">errTaskDropped</span><span class="sxs-lookup"><span data-stu-id="b640a-114">errTaskDropped</span></span>  <br/> |<span data-ttu-id="b640a-115">-106</span><span class="sxs-lookup"><span data-stu-id="b640a-115">-106</span></span>  <br/> |<span data-ttu-id="b640a-116">**ErrTerm** 関数によって返され、一部のデータベース ページとトランザクション ログ ファイルがチェックされなかったことや、検証中にエラーが発生したことを示します。</span><span class="sxs-lookup"><span data-stu-id="b640a-116">Returned by the **ErrTerm** function to indicate that not all database pages and transaction log files were checked, or that errors were encountered during the verification.</span></span>  <br/> |
|<span data-ttu-id="b640a-117">errRequiredLogFilesMissing ありません</span><span class="sxs-lookup"><span data-stu-id="b640a-117">errRequiredLogFilesMissing</span></span>  <br/> |<span data-ttu-id="b640a-118">-543</span><span class="sxs-lookup"><span data-stu-id="b640a-118">-543</span></span>  <br/> |<span data-ttu-id="b640a-119">データベースをクリーン シャットダウン状態にするために必要な 1 つ以上のログ ファイルがログ ファイル パスに見つからなかったか、指定された 3 文字のベース名がありませんでした。</span><span class="sxs-lookup"><span data-stu-id="b640a-119">One or more log files that are required to bring the database to a clean-shutdown state was not found in the log file path, or did not have the specified three-letter base name.</span></span>  <br/> |
|<span data-ttu-id="b640a-120">errInvalidParameter</span><span class="sxs-lookup"><span data-stu-id="b640a-120">errInvalidParameter</span></span>  <br/> |<span data-ttu-id="b640a-121">-1003</span><span class="sxs-lookup"><span data-stu-id="b640a-121">-1003</span></span>  <br/> |<span data-ttu-id="b640a-122">関数に渡された 1 つ以上のパラメーターが正しくありません。</span><span class="sxs-lookup"><span data-stu-id="b640a-122">One or more parameters that were passed to the function were invalid.</span></span>  <br/> |
|<span data-ttu-id="b640a-123">errOutOfMemory</span><span class="sxs-lookup"><span data-stu-id="b640a-123">errOutOfMemory</span></span>  <br/> |<span data-ttu-id="b640a-124">-1011</span><span class="sxs-lookup"><span data-stu-id="b640a-124">-1011</span></span>  <br/> |<span data-ttu-id="b640a-125">メモリ不足のため、要求された操作を完了できませんでした。</span><span class="sxs-lookup"><span data-stu-id="b640a-125">Insufficient memory was available to complete the requested operation.</span></span>  <br/> |
|<span data-ttu-id="b640a-126">errReadVerifyFailure</span><span class="sxs-lookup"><span data-stu-id="b640a-126">errReadVerifyFailure</span></span>  <br/> |<span data-ttu-id="b640a-127">-1018</span><span class="sxs-lookup"><span data-stu-id="b640a-127">-1018</span></span>  <br/> |<span data-ttu-id="b640a-128">データベース ページに格納されているチェックサムが、予期されるチェックサムと一致しません。</span><span class="sxs-lookup"><span data-stu-id="b640a-128">The checksum that is stored on a database page does not match its expected checksum.</span></span>  <br/> |
|<span data-ttu-id="b640a-129">errTooManyActiveUsers</span><span class="sxs-lookup"><span data-stu-id="b640a-129">errTooManyActiveUsers</span></span>  <br/> |<span data-ttu-id="b640a-130">-1059</span><span class="sxs-lookup"><span data-stu-id="b640a-130">-1059</span></span>  <br/> |<span data-ttu-id="b640a-131">オブジェクトの使用中に、**ErrTerm** 関数が呼び出されました。</span><span class="sxs-lookup"><span data-stu-id="b640a-131">The **ErrTerm** function was called while the object was still being used.</span></span> <span data-ttu-id="b640a-132">**ErrTerm** が、**ErrCheckDbPages** や **ErrCheckLogFiles** が返される前に呼び出されると、この状況が生じることがあります。</span><span class="sxs-lookup"><span data-stu-id="b640a-132">This can occur if **ErrTerm** is called before **ErrCheckDbPages** or **ErrCheckLogFiles** has returned.</span></span>  <br/> |
   
## <a name="requirements"></a><span data-ttu-id="b640a-133">Requirements</span><span class="sxs-lookup"><span data-stu-id="b640a-133">Requirements</span></span>

<span data-ttu-id="b640a-134">Exchange Server 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b640a-134">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="b640a-135">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="b640a-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

