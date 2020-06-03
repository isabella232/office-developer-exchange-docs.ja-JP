---
title: ServerVersion (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a
description: ServerVersion 要素は、Microsoft Exchange Server を実行しているコンピューターのバージョン番号を表します。
ms.openlocfilehash: 3ef531a69d2dd00ee9784c9eb191684ce517e842
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461969"
---
# <a name="serverversion-pox"></a><span data-ttu-id="6a16b-103">ServerVersion (POX)</span><span class="sxs-lookup"><span data-stu-id="6a16b-103">ServerVersion (POX)</span></span>

<span data-ttu-id="6a16b-104">**ServerVersion**要素は、Microsoft Exchange Server を実行しているコンピューターのバージョン番号を表します。</span><span class="sxs-lookup"><span data-stu-id="6a16b-104">The **ServerVersion** element represents the version number of the computer that is running Microsoft Exchange Server.</span></span> 
  
- [<span data-ttu-id="6a16b-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="6a16b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="6a16b-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="6a16b-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="6a16b-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="6a16b-107">Account (POX)</span></span>](account-pox.md)
- [<span data-ttu-id="6a16b-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="6a16b-108">Protocol (POX)</span></span>](protocol-pox.md)
- [<span data-ttu-id="6a16b-109">ServerVersion (POX)</span><span class="sxs-lookup"><span data-stu-id="6a16b-109">ServerVersion (POX)</span></span>](serverversion-pox.md)
  
```xml
<ServerVersion/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="6a16b-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6a16b-110">Attributes and elements</span></span>

<span data-ttu-id="6a16b-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a16b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a16b-112">属性</span><span class="sxs-lookup"><span data-stu-id="6a16b-112">Attributes</span></span>

<span data-ttu-id="6a16b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6a16b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a16b-114">子要素</span><span class="sxs-lookup"><span data-stu-id="6a16b-114">Child elements</span></span>

<span data-ttu-id="6a16b-115">なし。</span><span class="sxs-lookup"><span data-stu-id="6a16b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a16b-116">親要素</span><span class="sxs-lookup"><span data-stu-id="6a16b-116">Parent elements</span></span>

|<span data-ttu-id="6a16b-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="6a16b-117">**Element**</span></span>|<span data-ttu-id="6a16b-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a16b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a16b-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="6a16b-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="6a16b-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6a16b-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6a16b-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6a16b-121">Text value</span></span>

<span data-ttu-id="6a16b-122">Text 値は、Exchange サーバーのバージョン番号を表します。</span><span class="sxs-lookup"><span data-stu-id="6a16b-122">The text value represents the Exchange server version number.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6a16b-123">注釈</span><span class="sxs-lookup"><span data-stu-id="6a16b-123">Remarks</span></span>

<span data-ttu-id="6a16b-124">**ServerVersion**の値は、 [Type (POX)](type-pox.md)要素が EXCH または EXPR と等しい場合にのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="6a16b-124">The **ServerVersion** value is only valid if the [Type (POX)](type-pox.md) element is equal to EXCH or EXPR.</span></span> <span data-ttu-id="6a16b-125">**ServerVersion**の値は、サーバーの MajorVersion、MinorVersion、および MajorBuildNumber を含む16進数値です。</span><span class="sxs-lookup"><span data-stu-id="6a16b-125">The **ServerVersion** value is a hexadecimal number that contains the MajorVersion, MinorVersion, and MajorBuildNumber of the server.</span></span> 
  
## <a name="example"></a><span data-ttu-id="6a16b-126">例</span><span class="sxs-lookup"><span data-stu-id="6a16b-126">Example</span></span>

<span data-ttu-id="6a16b-127">次の例では、自動検出応答で返される**ServerVersion**値を取得して、MajorVersion、MinorVersion、および MajorBuildNumber を取得して表示します。</span><span class="sxs-lookup"><span data-stu-id="6a16b-127">The following example coverts a **ServerVersion** value that is returned in an Autodiscover response to obtain and display the MajorVersion, MinorVersion, and MajorBuildNumber.</span></span> <span data-ttu-id="6a16b-128">この例では、 **ServerVersion**値に16進数の値を入力できるようにします。</span><span class="sxs-lookup"><span data-stu-id="6a16b-128">This example enables you to enter a hexadecimal value for the **ServerVersion** value.</span></span> <span data-ttu-id="6a16b-129">**ServerVersion**値が入力されていない場合は、既定の**ServerVersion**値738180da が使用されます。</span><span class="sxs-lookup"><span data-stu-id="6a16b-129">If no **ServerVersion** value is entered, a default **ServerVersion** value of 738180DA is used.</span></span> 
  
```csharp
static void Main(string[] args)
{
    // Convert a ServerVersion value that is returned from an Autodiscover request.
    // The value is a hex value and can be converted to the MajorVersion, MinorVersion,
    // and MajorBuildNumber.
    Console.WriteLine("Enter ServerVersion returned from the Autodiscover (eg. 738180DA) and Enter.");
    Console.WriteLine("To use the default ServerVersion of 738180DA, just hit Enter.");
    // Get the hexadecimal ServerVersion value.
    string serverversionhex = Console.ReadLine();
    // If nothing is entered, use the default server version of "738180DA"
    if (serverversionhex == "")
    {
        serverversionhex = "738180DA";
    }
    Console.WriteLine("ServerVersion (Hex) = " + serverversionhex);
    string serverversionbinary = Convert.ToString(Convert.ToInt32(serverversionhex, 16), 2);
    // The ServerVersion (binary) should be 32 bits in length. If the 
    // server version in binary is a length of 31 characters, the leading
    // zero has been removed in the conversion process. Put the missing zero back.
    if (serverversionbinary.Length == 31)
    {
        serverversionbinary = String.Concat("0", serverversionbinary);
    }
    Console.WriteLine("ServerVersion (bin) = " + serverversionbinary);
    // The first 4 bits represent a number used for comparison against  
    // older version number structures. You can ignore this.
    // The next 6 bits represent the major version number.
    int majorversion = Convert.ToInt32(serverversionbinary.Substring(4, 6), 2);
    Console.WriteLine("MajorVersion: " + majorversion);
    // The next 6 bits represent the minor version number.
    int minorversion = Convert.ToInt32(serverversionbinary.Substring(10, 6), 2);
    Console.WriteLine("MinorVersion: " + minorversion);
    
    // The next bit represent a flag - you can ignore this.
    // The next 15 bits represent the major build number.
    int majorbuild = Convert.ToInt32(serverversionbinary.Substring(17, 15), 2);
    Console.WriteLine("MajorBuildVersion: " + majorbuild);
    Console.WriteLine("\n\nPress any key to continue");
    Console.ReadKey();
}
```

## <a name="see-also"></a><span data-ttu-id="6a16b-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a16b-130">See also</span></span>

- [<span data-ttu-id="6a16b-131">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="6a16b-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

