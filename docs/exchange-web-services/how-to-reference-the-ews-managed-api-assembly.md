---
title: EWS マネージ API アセンブリの参照
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 130990db-6297-42dc-9f5d-f68a2400872a
description: EWS マネージ API アセンブリを参照する方法についての情報を探します。
localization_priority: Priority
ms.openlocfilehash: d49091781da279d87a1eab35608f19ece43a0333
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527762"
---
# <a name="reference-the-ews-managed-api-assembly"></a>EWS マネージ API アセンブリの参照

EWS マネージ API アセンブリを参照する方法についての情報を探します。
  
EWS マネージ API は、Exchange Web サービス (EWS) を使用するアプリケーションを開発して拡張するためのシンプルかつフル機能を備えたインターフェイスを提供します。 EWS マネージ API アプリケーションを開発するために Visual Studio を使用しているにせよ、別のコード エディターを使用しているにせよ、EWS マネージ API アセンブリを参照する必要があります。 EWS マネージ API をまだインストールしていない場合は、必ず [API をダウンロード](https://aka.ms/ews-managed-api-readme)してください。
  
> [!NOTE]
> EWS マネージ API は、[GitHub](https://github.com/officedev/ews-managed-api) でオープンソース プロジェクトとして利用可能になりました。 オープン ソース ライブラリを使用して、以下のことができます。 
> - バグ修正と API の機能強化に貢献します。 
> - 公式のリリースで利用可能になる前に、修正プログラムや拡張機能を取得できます。 
> - API の最も包括的かつ最新の実装にアクセスして、参照として使用するか、新しいプラットフォームで新しいライブラリを作成します。
> 
>  GitHub を通した皆様の[貢献](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md)を歓迎いたします。 
  
## <a name="referencing-the-assembly"></a>アセンブリを参照する

参照を追加する最も一般的な方法は、Visual Studio を使用することです。他のエディターの使用を好む開発者がいることも理解していますので、Visual Studio を利用するための手順のほかに、コマンド ラインのコンパイラを利用するための手順も含めています。以下のコード例には同じ **using** ステートメントがあることにお気付きかもしれません。2 つの方法の違いは、コマンド ライン コンパイラはアセンブリ ファイルの場所が必要な点です。Visual Studio の参照は、これをバック グラウンドで処理します。 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a>Visual Studio を使用して参照を追加するには

1. Microsoft.Exchange.WebServices.dll のファイルおよび Microsoft.Exchange.WebServices.xml のファイルを任意のフォルダーに配置します。 既定では、ファイルは `C:\Program Files\Microsoft\Exchange\Web Services\2.0\` にインストールされますが、ファイルはお使いのコンピューターの任意の場所に保存することができます。
    
2. Visual Studio のソリューション エクスプローラー ウィンドウで、**[参照]** を選択してから、**[参照の追加]** を選択します。これにより、[参照の追加] ウィンドウが開きます。
    
3. [参照の追加] ウィンドウで **[参照]** タブに移動し、Microsoft.Exchange.WebServices.dll ファイルの場所を参照して、**[OK]** を選択します。  
    
4. アプリケーション内で EWS マネージ API を使用するには、**Microsoft.Exchange.WebServices.Data** 名前空間に **using** ステートメントを追加します。 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a>コマンド ライン コンパイラを使用して、参照を追加し、アプリケーションをビルドする

1. Microsoft.Exchange.WebServices.dll ファイルを任意のフォルダーに配置します。このフォルダーは、コンパイラの出力フォルダーになります。
    
2. ご使用のソース コード エディターで、**Microsoft.Exchange.WebServices.Data** 名前空間のソース コードに **using** ステートメントを追加します。 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. コマンド ライン コンパイラを実行してアプリケーションをビルドします。次のコマンドは、.NET Framework の C# コンパイラを使用して、ソース コード ファイル "program.cs" で定義されている Windows アプリケーションをビルドします。ここでは、コンパイラが既定のインストール ディレクトリ内にあり、Microsoft.Exchange.WebServices.dll ファイルが、"build" という名前の現在のディレクトリのサブディレクトリにあると想定しています。
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a>関連項目

- [EWS マネージ API クライアント アプリケーションの概要](get-started-with-ews-managed-api-client-applications.md)    
- [Exchange アプリケーションの開発環境をセットアップする](setting-up-your-exchange-application-development-environment.md)   
- [EWS マネージ API を使用して EWS と通信する](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

