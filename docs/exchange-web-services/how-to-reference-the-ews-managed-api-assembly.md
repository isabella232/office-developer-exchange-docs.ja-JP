---
title: EWS マネージ API アセンブリの参照
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 130990db-6297-42dc-9f5d-f68a2400872a
description: EWS マネージ API アセンブリを参照する方法についての情報を探します。
ms.openlocfilehash: a08ce43d139440186f611049fa1e457ea44f0362
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353687"
---
# <a name="reference-the-ews-managed-api-assembly"></a><span data-ttu-id="f54b4-103">EWS マネージ API アセンブリの参照</span><span class="sxs-lookup"><span data-stu-id="f54b4-103">How to: Reference the EWS Managed API assembly</span></span>

<span data-ttu-id="f54b4-104">EWS マネージ API アセンブリを参照する方法についての情報を探します。</span><span class="sxs-lookup"><span data-stu-id="f54b4-104">Find information about how to reference the EWS Managed API assembly.</span></span>
  
<span data-ttu-id="f54b4-105">EWS マネージ API は、Exchange Web サービス (EWS) を使用するアプリケーションを開発して拡張するためのシンプルかつフル機能を備えたインターフェイスを提供します。</span><span class="sxs-lookup"><span data-stu-id="f54b4-105">The EWS Managed API provides a simple and full-featured interface for developing and extending applications that use Exchange Web Services (EWS).</span></span> <span data-ttu-id="f54b4-106">EWS マネージ API アプリケーションを開発するために Visual Studio を使用しているにせよ、別のコード エディターを使用しているにせよ、EWS マネージ API アセンブリを参照する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f54b4-106">The EWS Managed API provides a simple and full-featured interface for developing and extending applications that use Exchange Web Services (EWS). Whether you are using Visual Studio or another code editor to develop your EWS Managed API application, you will need to make a reference to the EWS Managed API assembly. If you haven’t installed the EWS Managed API already, be sure to download the APIhttp://aka.ms/ews-managed-api-readme.</span></span> <span data-ttu-id="f54b4-107">EWS マネージ API をまだインストールしていない場合は、必ず [API をダウンロード](http://aka.ms/ews-managed-api-readme)してください。</span><span class="sxs-lookup"><span data-stu-id="f54b4-107">If you haven't installed the EWS Managed API already, be sure to [download the API](http://aka.ms/ews-managed-api-readme).</span></span>
  
> [!NOTE]
> <span data-ttu-id="f54b4-108">EWS マネージ API は、[GitHub](https://github.com/officedev/ews-managed-api) でオープンソース プロジェクトとして利用可能になりました。</span><span class="sxs-lookup"><span data-stu-id="f54b4-108">The EWS Managed API is now available as an open source project on  GitHub http://aka.ms/ews-managed-api-github . You can use the open source library to:</span></span> <span data-ttu-id="f54b4-109">オープン ソース ライブラリを使用して、以下のことができます。</span><span class="sxs-lookup"><span data-stu-id="f54b4-109">You can use the open source library to:</span></span> 
> - <span data-ttu-id="f54b4-110">バグ修正と API の機能強化に貢献します。</span><span class="sxs-lookup"><span data-stu-id="f54b4-110">Contribute bug fixes and enhancements to the API.</span></span> 
> - <span data-ttu-id="f54b4-111">公式のリリースで利用可能になる前に、修正プログラムや拡張機能を取得できます。</span><span class="sxs-lookup"><span data-stu-id="f54b4-111">Get fixes and enhancements before they are available in an official release.</span></span> 
> - <span data-ttu-id="f54b4-112">API の最も包括的かつ最新の実装にアクセスし、それを参照用として使用するか、それを新しいプラットフォーム上の新しいライブラリを作成するために使用します。</span><span class="sxs-lookup"><span data-stu-id="f54b4-112">Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms.</span></span>
> 
>  <span data-ttu-id="f54b4-113">GitHub を通した皆様の[貢献](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md)を歓迎いたします。</span><span class="sxs-lookup"><span data-stu-id="f54b4-113">We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="referencing-the-assembly"></a><span data-ttu-id="f54b4-114">アセンブリを参照する</span><span class="sxs-lookup"><span data-stu-id="f54b4-114">Referencing the assembly</span></span>

<span data-ttu-id="f54b4-p103">参照を追加する最も一般的な方法は、Visual Studio を使用することです。他のエディターの使用を好む開発者がいることも理解していますので、Visual Studio を利用するための手順のほかに、コマンド ラインのコンパイラを利用するための手順も含めています。以下のコード例には同じ **using** ステートメントがあることにお気付きかもしれません。2 つの方法の違いは、コマンド ライン コンパイラはアセンブリ ファイルの場所が必要な点です。Visual Studio の参照は、これをバック グラウンドで処理します。</span><span class="sxs-lookup"><span data-stu-id="f54b4-p103">The most common way to add a reference is to use Visual Studio. We know that some developers out there like to use other editors, so we are including instructions for using the command-line compiler as well as instructions for using Visual Studio. You might notice that the code examples that follow have the same **using** statements. The difference between the two methods is that the command-line compiler needs the location of the assembly file. The Visual Studio reference handles this for you behind the scenes.</span></span> 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a><span data-ttu-id="f54b4-120">Visual Studio を使用して参照を追加するには</span><span class="sxs-lookup"><span data-stu-id="f54b4-120">To add a reference by using Visual Studio</span></span>

1. <span data-ttu-id="f54b4-121">Microsoft.Exchange.WebServices.dll のファイルおよび Microsoft.Exchange.WebServices.xml のファイルを任意のフォルダーに配置します。</span><span class="sxs-lookup"><span data-stu-id="f54b4-121">Put the Microsoft.Exchange.WebServices.dll file and the Microsoft.Exchange.WebServices.xml file into a folder of your choice. By default, the files are installed in C:\Program Files\Microsoft\Exchange\Web Services\2.0\, but you can store the files anywhere on your computer.</span></span> <span data-ttu-id="f54b4-122">既定では、ファイルは `C:\Program Files\Microsoft\Exchange\Web Services\2.0\` にインストールされますが、ファイルはお使いのコンピューターの任意の場所に保存することができます。</span><span class="sxs-lookup"><span data-stu-id="f54b4-122">By default, the files are installed in  `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, but you can store the files anywhere on your computer.</span></span>
    
2. <span data-ttu-id="f54b4-p105">Visual Studio のソリューション エクスプローラー ウィンドウで、**[参照]** を選択してから、**[参照の追加]** を選択します。これにより、[参照の追加] ウィンドウが開きます。</span><span class="sxs-lookup"><span data-stu-id="f54b4-p105">In the Solution Explorer pane in Visual Studio, select **References**, and then choose **Add Reference**. This opens the Add Reference window.</span></span>
    
3. <span data-ttu-id="f54b4-125">[参照の追加] ウィンドウで **[参照]** タブに移動し、Microsoft.Exchange.WebServices.dll ファイルの場所を参照して、**[OK]** を選択します。 </span><span class="sxs-lookup"><span data-stu-id="f54b4-125">In the Add Reference window, navigate to the **Browse** tab, browse to the location of the Microsoft.Exchange.WebServices.dll file, select that file, and then select **OK**.</span></span> 
    
4. <span data-ttu-id="f54b4-126">アプリケーション内で EWS マネージ API を使用するには、**Microsoft.Exchange.WebServices.Data** 名前空間に **using** ステートメントを追加します。</span><span class="sxs-lookup"><span data-stu-id="f54b4-126">To use the EWS Managed API in your application, add a **using** statement for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a><span data-ttu-id="f54b4-127">コマンド ライン コンパイラを使用して、参照を追加し、アプリケーションをビルドする</span><span class="sxs-lookup"><span data-stu-id="f54b4-127">To add a reference and build your application with the command-line compiler</span></span>

1. <span data-ttu-id="f54b4-p106">Microsoft.Exchange.WebServices.dll ファイルを任意のフォルダーに配置します。このフォルダーは、コンパイラの出力フォルダーになります。</span><span class="sxs-lookup"><span data-stu-id="f54b4-p106">Put the Microsoft.Exchange.WebServices.dll file into a folder of your choice. This folder will be the output folder for the compiler.</span></span>
    
2. <span data-ttu-id="f54b4-130">ご使用のソース コード エディターで、**Microsoft.Exchange.WebServices.Data** 名前空間のソース コードに **using** ステートメントを追加します。</span><span class="sxs-lookup"><span data-stu-id="f54b4-130">In your source code editor, add a **using** statement to the source code for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. <span data-ttu-id="f54b4-p107">コマンド ライン コンパイラを実行してアプリケーションをビルドします。次のコマンドは、.NET Framework の C# コンパイラを使用して、ソース コード ファイル "program.cs" で定義されている Windows アプリケーションをビルドします。ここでは、コンパイラが既定のインストール ディレクトリ内にあり、Microsoft.Exchange.WebServices.dll ファイルが、"build" という名前の現在のディレクトリのサブディレクトリにあると想定しています。</span><span class="sxs-lookup"><span data-stu-id="f54b4-p107">Run the command-line compiler to build the application. The following command uses the .NET Framework C# compiler to build the Windows application defined in the source code file "program.cs". It assumes that the compiler is located in the default installation directory and that the Microsoft.Exchange.WebServices.dll file is in a subdirectory of the current directory named "build".</span></span>
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a><span data-ttu-id="f54b4-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="f54b4-134">See also</span></span>

- [<span data-ttu-id="f54b4-135">EWS マネージ API クライアント アプリケーションの概要</span><span class="sxs-lookup"><span data-stu-id="f54b4-135">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)    
- [<span data-ttu-id="f54b4-136">Exchange アプリケーションの開発環境をセットアップする</span><span class="sxs-lookup"><span data-stu-id="f54b4-136">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="f54b4-137">EWS マネージ API を使用して EWS と通信する</span><span class="sxs-lookup"><span data-stu-id="f54b4-137">How to: Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

