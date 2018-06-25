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
# <a name="reference-the-ews-managed-api-assembly"></a>EWS のマネージ API のアセンブリを参照します。

EWS マネージ API のアセンブリを参照する方法について、情報を見つけます。
  
EWS のマネージ API では、開発と、Exchange Web サービス (EWS) を使用するアプリケーションを拡張するためのシンプルかつフル機能を備えたインターフェイスを提供します。 EWS マネージ API アプリケーションを開発する Visual Studio または別のコード エディターを使用しているかどうかは、EWS のマネージ API のアセンブリへの参照を作成する必要があります。 EWS のマネージ API を既にインストールしていない場合、は、 [API をダウンロード](http://aka.ms/ews-managed-api-readme)することを確認します。
  
> [!NOTE]
>  [!メモ]  EWS マネージ API が、 [GitHub](https://github.com/officedev/ews-managed-api) のオープン ソース プロジェクトとして利用できるようになりました。オープン ソース ライブラリを使用して、次のことができます。 >  バグ修正と API の機能強化に貢献します。 >  公式のリリースで利用可能になる前に、修正プログラムや拡張機能を取得できます。 >  API の最も包括的かつ最新の実装にアクセスして、参照として使用するか、新しいプラットフォームで新しいライブラリを作成します。 >  GitHub による [貢献](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md)を歓迎いたします。 
  
## <a name="referencing-the-assembly"></a>アセンブリを参照する

参照を追加する最も一般的な方法では、Visual Studio を使用します。 ように、Visual Studio を使用するため、コマンド ライン コンパイラと同様の手順を使用する方法について、他のエディターを使用するを好むことを開発者が理解しています。 同じ**を使用して**ステートメントを以下のコード例があることがわかります可能性があります。 2 つの方法の違いは、コマンド ライン コンパイラ アセンブリ ファイルの場所が必要であります。 Visual Studio 参照する処理はバック グラウンドでします。 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a>Visual Studio を使用して参照を追加するには

1. Microsoft.Exchange.WebServices.dll ファイルおよび Microsoft.Exchange.WebServices.xml ファイルを任意のフォルダーに配置します。 既定では、ファイルがインストールされている`C:\Program Files\Microsoft\Exchange\Web Services\2.0\`、お使いのコンピューターの任意の場所にファイルを保存することです。
    
2. Visual Studio でソリューション エクスプ ローラー ウィンドウで**参照**を選択し、**参照の追加**します。 [参照の追加] ウィンドウが開きます。
    
3. [参照の追加] ウィンドウで、 **[参照**] タブに移動、Microsoft.Exchange.WebServices.dll ファイルの場所を参照して、そのファイルを選択し、 **[ok]** を選択し。 
    
4. EWS のマネージ API をアプリケーションで使用するには、 **Microsoft.Exchange.WebServices.Data**名前空間の**using**ステートメントを追加します。 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a>コマンド ライン コンパイラを使用して参照を追加し、アプリケーションをビルドするには

1. Microsoft.Exchange.WebServices.dll ファイルを任意のフォルダーに配置します。このフォルダーは、コンパイラの出力フォルダーになります。
    
2. ソース コード エディターでは、 **Microsoft.Exchange.WebServices.Data**名前空間をソース コードに**using**ステートメントを追加します。 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. コマンド ライン コンパイラを実行してアプリケーションをビルドします。次のコマンドは、.NET Framework の C# コンパイラを使用して、ソース コード ファイル "program.cs" で定義されている Windows アプリケーションをビルドします。ここでは、コンパイラが既定のインストール ディレクトリ内にあり、Microsoft.Exchange.WebServices.dll ファイルが、"build" という名前の現在のディレクトリのサブディレクトリにあると想定しています。
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a>関連項目

- [EWS マネージ API クライアント アプリケーションの概要](get-started-with-ews-managed-api-client-applications.md)    
- [Exchange アプリケーションの開発環境を設定します。](setting-up-your-exchange-application-development-environment.md)   
- [EWS のマネージ API を使用して通信 EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

