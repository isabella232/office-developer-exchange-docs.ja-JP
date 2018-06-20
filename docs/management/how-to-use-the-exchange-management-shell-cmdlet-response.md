---
title: Exchange 管理シェル コマンドレットの応答を使用します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dac8e526-11c6-4c2e-b9a2-f016b1fc738a
description: Exchange の管理アプリケーションで、Exchange 管理シェル コマンドレットからの応答を使用する方法について説明します。
ms.openlocfilehash: 5edf75afd556f67e815bc519c87586f2f62f057b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759194"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a><span data-ttu-id="7defb-103">Exchange 管理シェル コマンドレットの応答を使用します。</span><span class="sxs-lookup"><span data-stu-id="7defb-103">Use the Exchange Management Shell cmdlet response</span></span>

<span data-ttu-id="7defb-104">Exchange の管理アプリケーションで、Exchange 管理シェル コマンドレットからの応答を使用する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="7defb-104">Learn how to use the response from an Exchange Management Shell cmdlet in your Exchange managed application.</span></span>
  
<span data-ttu-id="7defb-105">**に適用されます:** オンライン交換 |Exchange Server 2013年 |Office 365</span><span class="sxs-lookup"><span data-stu-id="7defb-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="7defb-106">各 Exchange 管理シェル コマンドレットは、Exchange 管理シェル環境での任意のオブジェクトの整合性のとれたビューを提供する 1 つまたは複数の[PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx)インスタンスを返します。</span><span class="sxs-lookup"><span data-stu-id="7defb-106">Each Exchange Management Shell cmdlet returns one or more [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) instances that provide a consistent view of any object in the Exchange Management Shell environment.</span></span> <span data-ttu-id="7defb-107">**PSObject**インスタンスのプロパティを使用して、基になる Exchange Server 2013 API オブジェクトのプロパティ値を取得する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="7defb-107">This article provides information about how to use the properties of a **PSObject** instance to return the property values of the underlying Exchange Server 2013 API object.</span></span> 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a><span data-ttu-id="7defb-108">コマンドレットの応答を使用するための前提条件</span><span class="sxs-lookup"><span data-stu-id="7defb-108">Prerequisites for using cmdlet responses</span></span>
<span data-ttu-id="7defb-109"><a name="prerequisites_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="7defb-109"></span></span>

<span data-ttu-id="7defb-110">コマンドレットの応答を使用するには、 **System.Automation.Management**名前空間への参照が必要です。</span><span class="sxs-lookup"><span data-stu-id="7defb-110">To use cmdlet responses, you need a reference to the **System.Automation.Management** namespace.</span></span> 
  
> [!NOTE]
>  <span data-ttu-id="7defb-p102">Visual Studio を使用してアプリケーションを作成するときには、System.Mangagement.Automation.dll アセンブリの参照をプロジェクトに追加する必要があります。アセンブリは次の場所のいずれかにあります。</span><span class="sxs-lookup"><span data-stu-id="7defb-p102">When you are using Visual Studio to create an application, you must add a reference to the System.Mangagement.Automation.dll assembly to the project. You can find the assembly in one of the following locations:</span></span> 
> - <span data-ttu-id="7defb-113">オペレーティング システムが Windows XP および Windows Vista の場合、Windows PowerShell のインストール ディレクトリ ($PSHOME)。</span><span class="sxs-lookup"><span data-stu-id="7defb-113">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span> 
> - <span data-ttu-id="7defb-114">オペレーティング システムが Windows 7 および Windows 8 の場合は次のフォルダー:Windows\assembly\GAC_MSIL\System.Management.Automation。</span><span class="sxs-lookup"><span data-stu-id="7defb-114">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
## <a name="windows-powershell-remote-runspace"></a><span data-ttu-id="7defb-115">Windows PowerShell のリモート実行空間</span><span class="sxs-lookup"><span data-stu-id="7defb-115">Windows PowerShell remote runspace</span></span>
<span data-ttu-id="7defb-116"><a name="usingremoterunspace_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="7defb-116"></span></span>

<span data-ttu-id="7defb-p103">Exchange 管理シェルでは、ローカル サーバーで実行されるコマンドであっても、すべてのコマンドに対して Windows PowerShell のリモート機能を使用します。その結果、Exchange 管理シェル コマンドレットからの応答は、すべてシリアル化された XML となります。つまり、その応答オブジェクトは、応答を生成するために使用した Exchange オブジェクトの種類は示しますが、Exchange オブジェクトの種類には型変換されません。代わりに、ユーザーご自身で、応答オブジェクトが公開するプロパティ バッグを使用して、Exchange オブジェクトの型から値を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7defb-p103">The Exchange Management Shell uses remote Windows PowerShell features for all commands, even commands that are run on the local server. As a result, all responses from Exchange Management Shell cmdlets are serialized XML. This means that although the response object indicates the Exchange object type that was used to generate the response, the response object cannot be cast to the Exchange object type; instead, you must use the property bag that is exposed by the response object to obtain the values from the Exchange object type.</span></span>
  
<span data-ttu-id="7defb-p104">応答オブジェクトのプロパティ バッグには、Exchange オブジェクト種類のパブリック プロパティまたはメソッドのごとにキー/値のペアが含まれています。応答オブジェクトには、基になる Exchange オブジェクト型の名前が含まれています。ユーザーはこの名前を使用して応答オブジェクトが表す Exchange オブジェクト型を決定し、プロパティを適切に抽出できます。ユーザーが適切に管理される型にプロパティ値を変換できるように、プロパティ バッグ内の各値には型情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="7defb-p104">The property bag in the response object contains a key/value pair for each public property or method in the Exchange object type. The response object contains the name of the underlying Exchange object type; you can use this name to determine the Exchange object type that is represented by the response object so that you can extract the appropriate property. Each value in the property bag also includes type information so that you can cast the property value to the appropriate managed type.</span></span>
  
## <a name="use-the-cmdlet-response"></a><span data-ttu-id="7defb-123">コマンドレット応答を使用する</span><span class="sxs-lookup"><span data-stu-id="7defb-123">Use the cmdlet response</span></span>
<span data-ttu-id="7defb-124"><a name="usingPSObject_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="7defb-124"></span></span>

<span data-ttu-id="7defb-125">[PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx)クラスを基になる Exchange 2013 の API のオブジェクトの値を含む、次の 3 つパブリック プロパティを公開する:[プロパティ](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.properties%28VS.85%29.aspx)、[メソッド](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.methods%28VS.85%29.aspx)、および[メンバー](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.members%28VS.85%29.aspx)。</span><span class="sxs-lookup"><span data-stu-id="7defb-125">The [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) class exposes the following three public properties that contain the values of the underlying Exchange 2013 API object: [Properties](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [Methods](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.methods%28VS.85%29.aspx), and [Members](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.members%28VS.85%29.aspx).</span></span> <span data-ttu-id="7defb-126">Exchange 2013 API オブジェクトによって公開されている各プロパティには、**プロパティ**と**メンバー**のプロパティで対応するキー/値のペアがあります。</span><span class="sxs-lookup"><span data-stu-id="7defb-126">Each property that is exposed by the Exchange 2013 API object has a corresponding key/value pair in the **Properties** and **Members** properties.</span></span> <span data-ttu-id="7defb-127">アプリケーションは、プロパティの値を取得するプロパティの名前を**Properties**コレクションのインデックスを作成できます。</span><span class="sxs-lookup"><span data-stu-id="7defb-127">Your application can index the **Properties** collection by the name of a property to retrieve the value of the property.</span></span> 
  
<span data-ttu-id="7defb-128">**PSObject**インスタンスの**型名**プロパティを使用するには**PSObject**のインスタンスによってカプセル化された基になる Exchange オブジェクトの種類を決定します。</span><span class="sxs-lookup"><span data-stu-id="7defb-128">You can use the **TypeNames** property of the **PSObject** instance to determine the type of the underlying Exchange object that is encapsulated by the **PSObject** instance.</span></span> <span data-ttu-id="7defb-129">**型名**のプロパティは、表される型のオブジェクトの階層を含む文字列のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7defb-129">The **TypeNames** property is a collection of strings that contains the object hierarchy of the represented type.</span></span> <span data-ttu-id="7defb-130">これらの名前を使用するには、適切なプロパティを抽出することができますように**PSObject**のインスタンスによって表されるオブジェクトを決定します。</span><span class="sxs-lookup"><span data-stu-id="7defb-130">You can use these names to determine the object that is represented by the **PSObject** instance so that you can extract the appropriate property.</span></span> 
  
<span data-ttu-id="7defb-131">次のコード例は、 **PSObject**インスタンスの**プロパティ**のコレクションの内容をコンソールに印刷するのには、コマンドレットの応答を使用します。</span><span class="sxs-lookup"><span data-stu-id="7defb-131">The following code example uses the cmdlet response to print the contents of the **Properties** collection of a **PSObject** instance on the console.</span></span> <span data-ttu-id="7defb-132">コード例では、 **System.Automation.Management**名前空間への参照が必要です。</span><span class="sxs-lookup"><span data-stu-id="7defb-132">The code example requires a reference to the **System.Automation.Management** namespace.</span></span> 
  
```cs
foreach (PSPropertyInfo propertyInfo in psObject.Properties)
{
    Console.WriteLine(string.Format("{0}: {1}",
        propertyInfo.Name, propertyInfo.Value);
}
```

<br/>

```vb
For Each PropertyInfo As PSProperty In ObjectInfo.Properties
    Console.WriteLine(String.Format("{0}: {1}", PropertyInfo.Name, PropertyInfo.Value))
Next

```

## <a name="see-also"></a><span data-ttu-id="7defb-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="7defb-133">See also</span></span>

- [<span data-ttu-id="7defb-134">Exchange 管理シェルのツールを作成します。</span><span class="sxs-lookup"><span data-stu-id="7defb-134">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="7defb-135">Exchange 管理シェルを使用してメール ユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="7defb-135">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

