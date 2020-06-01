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
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: b7c3517779eb07ef053c1dd4fa25544310fb3343
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455262"
---
# <a name="cchksgfilescmaxdbpersg-function"></a><span data-ttu-id="53695-103">CChkSGFiles.CMaxDbPerSG 関数</span><span class="sxs-lookup"><span data-stu-id="53695-103">CChkSGFiles.CMaxDbPerSG function</span></span>

<span data-ttu-id="53695-104">**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="53695-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="53695-105">1 つの Exchange サーバー ストレージ グループに許容されるデータベースの最大数を返します。</span><span class="sxs-lookup"><span data-stu-id="53695-105">Returns the maximum number of databases allowed in a single Exchange server storage group.</span></span>
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a><span data-ttu-id="53695-106">パラメーター</span><span class="sxs-lookup"><span data-stu-id="53695-106">Parameters</span></span>

<span data-ttu-id="53695-107">なし。</span><span class="sxs-lookup"><span data-stu-id="53695-107">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="53695-108">Return value</span><span class="sxs-lookup"><span data-stu-id="53695-108">Return value</span></span>

<span data-ttu-id="53695-109">指定した Exchange サーバーでストレージ グループごとに許容されるデータベースの最大数。</span><span class="sxs-lookup"><span data-stu-id="53695-109">The maximum number of databases that the specified Exchange server allows per storage group.</span></span> <span data-ttu-id="53695-110">ストレージグループは Exchange 2013 の一部ではないため、この関数は1を返します。</span><span class="sxs-lookup"><span data-stu-id="53695-110">Because storage groups are not part of Exchange 2013, this function returns 1.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="53695-111">注釈</span><span class="sxs-lookup"><span data-stu-id="53695-111">Remarks</span></span>

<span data-ttu-id="53695-112">**CCheckSGFiles** オブジェクトを使用すると唯一のストレージ グループに含まれるデータベース (およびトランザクション ログ ファイル) を検証できます。そのため、**CMaxDbPerSG** 関数から返される値もデータベースの最大数を表すことになります。これは、**CCheckSGFiles** クラスのインスタンスを使用することで確認できます。 </span><span class="sxs-lookup"><span data-stu-id="53695-112">You can use the **CCheckSGFiles** object to validate databases (and transaction log files) in only one storage group, so the value returned by the **CMaxDbPerSG** function also represents the maximum number of databases that you can check by using an instance of the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="53695-113">既定では、Exchange Server 2003 および Exchange Server 2007 では、ストレージグループごとに最大5つのデータベースが許可されていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="53695-113">Note that by default, Exchange Server 2003 and Exchange Server 2007 allow a maximum of five databases per storage group.</span></span>
  
## <a name="requirements"></a><span data-ttu-id="53695-114">Requirements</span><span class="sxs-lookup"><span data-stu-id="53695-114">Requirements</span></span>

<span data-ttu-id="53695-115">Exchange 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="53695-115">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="53695-116">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="53695-116">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

