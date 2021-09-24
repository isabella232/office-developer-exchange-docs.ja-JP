---
title: ServerVersion (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a
description: ServerVersion 要素は、サーバーで実行されているコンピューターのバージョン番号をMicrosoft Exchange Server。
ms.openlocfilehash: bc7f9daa62e628e41f7541a609550e90af211928
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527378"
---
# <a name="serverversion-pox"></a>ServerVersion (POX)

**ServerVersion 要素** は、サーバーで実行されているコンピューターのバージョン番号Microsoft Exchange Server。 
  
- [AutoDiscover (POX)](autodiscover-pox.md) 
- [Response (POX)](response-pox.md)
- [Account (POX)](account-pox.md)
- [Protocol (POX)](protocol-pox.md)
- [ServerVersion (POX)](serverversion-pox.md)
  
```xml
<ServerVersion/>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされている Microsoft Exchangeコンピューターにクライアントを接続するための仕様が含まれている。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、サーバーのバージョンExchangeを表します。
  
## <a name="remarks"></a>注釈

**ServerVersion の** 値は [、Type (POX)](type-pox.md)要素が EXCH または EXPR と等しい場合にのみ有効です。 **ServerVersion の** 値は、サーバーの MajorVersion、MinorVersion、および MajorBuildNumber を含む 16 進数です。 
  
## <a name="example"></a>例

次の例では、自動検出応答で返される **ServerVersion** 値をカバーし、MajorVersion、MinorVersion、および MajorBuildNumber を取得して表示します。 この例では **、ServerVersion** 値に 16 進値を入力できます。 **ServerVersion 値を入力** すると、既定の **ServerVersion** 値 738180DA が使用されます。 
  
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

## <a name="see-also"></a>関連項目

- [POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

