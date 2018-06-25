---
title: Exchange アプリケーションの開発環境をセットアップする
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 91b86e93-bdde-41c3-9680-45cf61420592
description: 開発環境をセットアップして、Exchange と通信する EWS アプリケーションを作成する方法について説明します。
ms.openlocfilehash: 0c7d4c6d37b28b6797bdb638930b8582f31ffc5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759183"
---
# <a name="setting-up-your-exchange-application-development-environment"></a>Exchange アプリケーションの開発環境をセットアップする

開発環境をセットアップして、Exchange と通信する EWS アプリケーションを作成する方法について説明します。
  
Exchange Web サービス (EWS) アプリケーションの作成を開始する前に、開発環境が、いくつかの最小要件を満たしているかどうかを確認する必要があります。 EWS 管理の API を.NET Framework アプリケーションでは、標準的なクライアント アクセス API を使用するには、アプリケーションを開発するか、自身での EWS を使用することができます、自動生成されたプロキシを使用せず。 EWS マネージ API を使用する一般に、ことを推奨します。できますの詳細を検索するのには[これら 2 つのオプションの違いを調べる](ews-client-design-overview-for-exchange.md)先を 1 つは、お客様に最適です。 
  
> [!NOTE]
>  [!メモ]  EWS マネージ API が、 [GitHub](https://github.com/officedev/ews-managed-api) のオープン ソース プロジェクトとして利用できるようになりました。オープン ソース ライブラリを使用して、次のことができます。 >  バグ修正と API の機能強化に貢献します。 >  公式のリリースで利用可能になる前に、修正プログラムや拡張機能を取得できます。 >  API の最も包括的かつ最新の実装にアクセスして、参照として使用するか、新しいプラットフォームで新しいライブラリを作成します。 >  GitHub による [貢献](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md)を歓迎いたします。 
  
## <a name="development-environment-for-the-ews-managed-api"></a>EWS マネージ API の開発環境
<a name="bk_EWSMA"> </a>

EWS のマネージ API アプリケーションを作成するには、次へのアクセスを必要があります。
  
- [EWS マネージ API](http://aka.ms/ews-managed-api-readme)。 
    
    お使いのコンピューターの任意の場所に EWS のマネージ API のファイルを格納することができます。プログラムの Files\Microsoft\Exchange\Web サービスで既定でインストールされる\\< バージョン番号\>フォルダー。
    
- Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2007 以降のバージョンの Exchange を実行している Exchange サーバー上のメールボックス。  
    
    [Office 365 サイト](http://office.microsoft.com/en-us/business/compare-office-365-for-business-plans-FX102918419.aspx#fbid=1tsGNIE7e3a)から、無料の試用版を含む、ビジネスのため、Exchange のオンラインの計画を取得できます。 メールボックスに接続するのには、ユーザー名とメールボックスに関連付けられているアカウントの資格情報が必要です。
    
- Visual Studio の Visual Studio 2005 以降のバージョンです。 現在 Visual Studio をお持ちでない場合は、 [Visual Studio 2010 Express](http://www.microsoft.com/visualstudio/eng/products/visual-studio-2010-express)の無料版をダウンロードできます。
    
- .NET Framework 3.5 以降の.NET Framework のバージョンです。 .NET Framework 3.5 は、 [Microsoft ダウンロード センター](http://go.microsoft.com/fwlink/?LinkId=191777)からダウンロードできます。
    
また、C# をある程度理解しておくと役立ちます。Visual Studio は C# だけでなく他の言語がサポートしていますが、EWS マネージ API で使用できるサンプル コードのほとんどは C# で記述されています。
  
## <a name="development-environment-for-ews"></a>EWS の開発環境
<a name="bk_EWS"> </a>

EWS を使用して、2 通りの方法でアプリケーションを開発できます。EWS を使用する最も簡単な方法は、XML 要求を含むテキスト ファイルを作成し、Exchange に送信する方法です。これを行うには、次のものが必要になります。  
  
- XML 要求を編集するためのメモ帳などの単純なテキスト エディター。任意のテキスト エディターが使用できますが、XMetal のような XML 構文の検証に役立つテキスト エディターを使用すると良いでしょう。
    
- Exchange と通信するために、SOAP XML の要求と応答を送受信できるツールまたはアプリケーション。
    
生の XML を使用する場合も XML の書式設定の基礎知識を習得するおくと便利です。
  
EWS を使用する 2 番目の方法は、自動生成されるプロキシを作成して、C# などの .NET 言語を使用した操作で作業できるようにする方法です。自動生成されるプロキシで操作するために必要なのものは次の通りです。
  
- 開始 Visual Studio 2005 では、プロキシ参照を作成すると、Visual Studio のバージョンです。 [Visual Studio 2010 Express](http://www.microsoft.com/visualstudio/eng/products/visual-studio-2010-express)の無料版をダウンロードすることができます。
    
- .NET Framework 2.0 以降の.NET Framework のバージョンです。 .NET Framework 3.5 は、 [Microsoft ダウンロード センター](http://go.microsoft.com/fwlink/?LinkId=191777)からダウンロードできます。
    
自動生成されたプロキシを使用する場合は、C# プログラミングの知識もします。
  
> [!NOTE]
> .NET Framework 開発者なら、お勧め EWS を開発するための自動生成されたプロキシではなく、EWS のマネージ API を使用します。 EWS のマネージ API のオブジェクト モデルは、自動生成されたプロキシ オブジェクト モデルよりも使いやすくします。 また、EWS のマネージ API では、[自動検出](autodiscover-for-exchange.md)を実装し、クライアント側のロジックが含まれています。 
  
## <a name="see-also"></a>関連項目


- [Exchange アプリケーションの開発環境を設定します。](setting-up-your-exchange-application-development-environment.md)
    
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
    
- [Exchange EWS へのアクセスを制御します。](how-to-control-access-to-ews-in-exchange.md)
    
- [EWS 交換用のオブジェクト モデルの生成](https://msdn.microsoft.com/en-us/library/jj190899)
    

