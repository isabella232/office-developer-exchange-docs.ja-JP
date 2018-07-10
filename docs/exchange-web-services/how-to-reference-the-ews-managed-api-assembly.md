---
title: EWS のマネージ API のアセンブリを参照します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 130990db-6297-42dc-9f5d-f68a2400872a
description: EWS マネージ API のアセンブリを参照する方法について、情報を見つけます。
ms.openlocfilehash: af7b1ec449c24e7fa4db89abb30e5ebc9f8d329e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759045"
---
# <a name="reference-the-ews-managed-api-assembly"></a><span data-ttu-id="1f89a-103">EWS のマネージ API のアセンブリを参照します。</span><span class="sxs-lookup"><span data-stu-id="1f89a-103">Reference the EWS Managed API assembly</span></span>

<span data-ttu-id="1f89a-104">EWS マネージ API のアセンブリを参照する方法について、情報を見つけます。</span><span class="sxs-lookup"><span data-stu-id="1f89a-104">Find information about how to reference the EWS Managed API assembly.</span></span>
  
<span data-ttu-id="1f89a-105">EWS のマネージ API では、開発と、Exchange Web サービス (EWS) を使用するアプリケーションを拡張するためのシンプルかつフル機能を備えたインターフェイスを提供します。</span><span class="sxs-lookup"><span data-stu-id="1f89a-105">The EWS Managed API provides a simple and full-featured interface for developing and extending applications that use Exchange Web Services (EWS).</span></span> <span data-ttu-id="1f89a-106">EWS マネージ API アプリケーションを開発する Visual Studio または別のコード エディターを使用しているかどうかは、EWS のマネージ API のアセンブリへの参照を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f89a-106">Whether you are using Visual Studio or another code editor to develop your EWS Managed API application, you will need to make a reference to the EWS Managed API assembly.</span></span> <span data-ttu-id="1f89a-107">EWS のマネージ API を既にインストールしていない場合、は、 [API をダウンロード](http://aka.ms/ews-managed-api-readme)することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1f89a-107">If you haven't installed the EWS Managed API already, be sure to [download the API](http://aka.ms/ews-managed-api-readme).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="1f89a-p102"> EWS マネージ API が、 [GitHub](https://github.com/officedev/ews-managed-api) のオープン ソース プロジェクトとして利用できるようになりました。オープン ソース ライブラリを使用して、次のことができます。 >  バグ修正と API の機能強化に貢献します。 >  公式のリリースで利用可能になる前に、修正プログラムや拡張機能を取得できます。 >  API の最も包括的かつ最新の実装にアクセスして、参照として使用するか、新しいプラットフォームで新しいライブラリを作成します。 >  GitHub による [貢献](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md)を歓迎いたします。</span><span class="sxs-lookup"><span data-stu-id="1f89a-p102">The EWS Managed API is now available as an open source project on [GitHub](https://github.com/officedev/ews-managed-api). You can use the open source library to: >  Contribute bug fixes and enhancements to the API. >  Get fixes and enhancements before they are available in an official release. >  Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms. >  We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="referencing-the-assembly"></a><span data-ttu-id="1f89a-113">アセンブリを参照する</span><span class="sxs-lookup"><span data-stu-id="1f89a-113">Referencing the assembly</span></span>

<span data-ttu-id="1f89a-114">参照を追加する最も一般的な方法では、Visual Studio を使用します。</span><span class="sxs-lookup"><span data-stu-id="1f89a-114">The most common way to add a reference is to use Visual Studio.</span></span> <span data-ttu-id="1f89a-115">ように、Visual Studio を使用するため、コマンド ライン コンパイラと同様の手順を使用する方法について、他のエディターを使用するを好むことを開発者が理解しています。</span><span class="sxs-lookup"><span data-stu-id="1f89a-115">We know that some developers out there like to use other editors, so we are including instructions for using the command-line compiler as well as instructions for using Visual Studio.</span></span> <span data-ttu-id="1f89a-116">同じ**を使用して**ステートメントを以下のコード例があることがわかります可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1f89a-116">You might notice that the code examples that follow have the same **using** statements.</span></span> <span data-ttu-id="1f89a-117">2 つの方法の違いは、コマンド ライン コンパイラ アセンブリ ファイルの場所が必要であります。</span><span class="sxs-lookup"><span data-stu-id="1f89a-117">The difference between the two methods is that the command-line compiler needs the location of the assembly file.</span></span> <span data-ttu-id="1f89a-118">Visual Studio 参照する処理はバック グラウンドでします。</span><span class="sxs-lookup"><span data-stu-id="1f89a-118">The Visual Studio reference handles this for you behind the scenes.</span></span> 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a><span data-ttu-id="1f89a-119">Visual Studio を使用して参照を追加するには</span><span class="sxs-lookup"><span data-stu-id="1f89a-119">To add a reference by using Visual Studio</span></span>

1. <span data-ttu-id="1f89a-120">Microsoft.Exchange.WebServices.dll ファイルおよび Microsoft.Exchange.WebServices.xml ファイルを任意のフォルダーに配置します。</span><span class="sxs-lookup"><span data-stu-id="1f89a-120">Put the Microsoft.Exchange.WebServices.dll file and the Microsoft.Exchange.WebServices.xml file into a folder of your choice.</span></span> <span data-ttu-id="1f89a-121">既定では、ファイルがインストールされている`C:\Program Files\Microsoft\Exchange\Web Services\2.0\`、お使いのコンピューターの任意の場所にファイルを保存することです。</span><span class="sxs-lookup"><span data-stu-id="1f89a-121">By default, the files are installed in  `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, but you can store the files anywhere on your computer.</span></span>
    
2. <span data-ttu-id="1f89a-122">Visual Studio でソリューション エクスプ ローラー ウィンドウで**参照**を選択し、**参照の追加**します。</span><span class="sxs-lookup"><span data-stu-id="1f89a-122">In the Solution Explorer pane in Visual Studio, select **References**, and then choose **Add Reference**.</span></span> <span data-ttu-id="1f89a-123">[参照の追加] ウィンドウが開きます。</span><span class="sxs-lookup"><span data-stu-id="1f89a-123">This opens the Add Reference window.</span></span>
    
3. <span data-ttu-id="1f89a-124">[参照の追加] ウィンドウで、 **[参照**] タブに移動、Microsoft.Exchange.WebServices.dll ファイルの場所を参照して、そのファイルを選択し、 **[ok]** を選択し。</span><span class="sxs-lookup"><span data-stu-id="1f89a-124">In the Add Reference window, navigate to the **Browse** tab, browse to the location of the Microsoft.Exchange.WebServices.dll file, select that file, and then select **OK**.</span></span> 
    
4. <span data-ttu-id="1f89a-125">EWS のマネージ API をアプリケーションで使用するには、 **Microsoft.Exchange.WebServices.Data**名前空間の**using**ステートメントを追加します。</span><span class="sxs-lookup"><span data-stu-id="1f89a-125">To use the EWS Managed API in your application, add a **using** statement for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a><span data-ttu-id="1f89a-126">コマンド ライン コンパイラを使用して参照を追加し、アプリケーションをビルドするには</span><span class="sxs-lookup"><span data-stu-id="1f89a-126">To add a reference and build your application with the command-line compiler</span></span>

1. <span data-ttu-id="1f89a-p106">Microsoft.Exchange.WebServices.dll ファイルを任意のフォルダーに配置します。このフォルダーは、コンパイラの出力フォルダーになります。</span><span class="sxs-lookup"><span data-stu-id="1f89a-p106">Put the Microsoft.Exchange.WebServices.dll file into a folder of your choice. This folder will be the output folder for the compiler.</span></span>
    
2. <span data-ttu-id="1f89a-129">ソース コード エディターでは、 **Microsoft.Exchange.WebServices.Data**名前空間をソース コードに**using**ステートメントを追加します。</span><span class="sxs-lookup"><span data-stu-id="1f89a-129">In your source code editor, add a **using** statement to the source code for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. <span data-ttu-id="1f89a-p107">コマンド ライン コンパイラを実行してアプリケーションをビルドします。次のコマンドは、.NET Framework の C# コンパイラを使用して、ソース コード ファイル "program.cs" で定義されている Windows アプリケーションをビルドします。ここでは、コンパイラが既定のインストール ディレクトリ内にあり、Microsoft.Exchange.WebServices.dll ファイルが、"build" という名前の現在のディレクトリのサブディレクトリにあると想定しています。</span><span class="sxs-lookup"><span data-stu-id="1f89a-p107">Run the command-line compiler to build the application. The following command uses the .NET Framework C# compiler to build the Windows application defined in the source code file "program.cs". It assumes that the compiler is located in the default installation directory and that the Microsoft.Exchange.WebServices.dll file is in a subdirectory of the current directory named "build".</span></span>
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a><span data-ttu-id="1f89a-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f89a-133">See also</span></span>

- [<span data-ttu-id="1f89a-134">EWS マネージ API クライアント アプリケーションの概要</span><span class="sxs-lookup"><span data-stu-id="1f89a-134">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)    
- [<span data-ttu-id="1f89a-135">Exchange アプリケーションの開発環境を設定します。</span><span class="sxs-lookup"><span data-stu-id="1f89a-135">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="1f89a-136">EWS のマネージ API を使用して通信 EWS</span><span class="sxs-lookup"><span data-stu-id="1f89a-136">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

