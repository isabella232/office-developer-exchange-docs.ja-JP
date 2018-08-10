---
title: Exchange アプリケーションの開発環境をセットアップする
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 91b86e93-bdde-41c3-9680-45cf61420592
description: 開発環境をセットアップして、Exchange と通信する EWS アプリケーションを作成する方法について説明します。
ms.openlocfilehash: 41664304eebf44d7985c774e260038eae4f23156
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353274"
---
# <a name="setting-up-your-exchange-application-development-environment"></a>Exchange アプリケーションの開発環境をセットアップする

開発環境をセットアップして、Exchange と通信する EWS アプリケーションを作成する方法について説明します。
  
Exchange Web サービス (EWS) アプリケーションの記述を開始する前に、開発環境がいくつかの最小要件を満たしているかどうかを確認する必要があります。 .NET Framework アプリケーション用の標準クライアント アクセス API である EWS マネージ API を使用して、アプリケーションを開発できます。また、自動生成されたプロキシ使用しているかどうかに関係なく、EWS をそれ自体で使用して、アプリケーションを開発できます。 通常は、EWS マネージ API を使用することをお勧めします。ただし、詳しく[これら 2 つのオプションの違いを調べて](ews-client-design-overview-for-exchange.md)、どちらが適切であるかを確認できます。 
  
> [!NOTE]
> EWS マネージ API は、[GitHub](https://github.com/officedev/ews-managed-api) でオープンソース プロジェクトとして利用可能になりました。 オープン ソース ライブラリを使用して、以下のことができます。 
> - バグ修正と API の機能強化に貢献します。 
> - 公式のリリースで利用可能になる前に、修正プログラムや拡張機能を取得できます。 
> - API の最も包括的かつ最新の実装にアクセスし、それを参照用として使用するか、それを新しいプラットフォーム上の新しいライブラリを作成するために使用します。
> 
>  GitHub を通した皆様の[貢献](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md)を歓迎いたします。 
  
## <a name="development-environment-for-the-ews-managed-api"></a>EWS マネージ API の開発環境
<a name="bk_EWSMA"> </a>

EWS マネージ API アプリケーションを作成するには、次にアクセスする必要があります。
  
- [EWS マネージ API](http://aka.ms/ews-managed-api-readme)。 
    
    EWS マネージ API ファイルはコンピューターの任意の場所に保存することができます。既定では、Files\Microsoft\Exchange\Web Services\\<version number\> フォルダーにインストールされます。
    
- Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2007 以降のバージョンの Exchange を実行している Exchange サーバー上のメールボックス。 
    
    [Office 365 サイト](http://office.microsoft.com/ja-JP/business/compare-office-365-for-business-plans-FX102918419.aspx#fbid=1tsGNIE7e3a)から、無料試用版を含むビジネス用 Exchange Online プランを入手できます。 メールボックスに接続するには、メールボックスに関連付けられているアカウントのユーザー名と資格情報が必要です。
    
- Visual Studio 2005 以降のいずれかのバージョンの Visual Studio。 現在、Visual Studio をお持ちでない場合は、[無料版](https://visualstudio.microsoft.com/)をダウンロードできます。
    
- .NET Framework 3.5 以降のいずれかのバージョンの .NET Framework。 .NET Framework 3.5 は、[Microsoft ダウンロード センター](http://go.microsoft.com/fwlink/?LinkId=191777)からダウンロードできます。
    
また、C# をある程度理解しておくと役立ちます。Visual Studio は C# だけでなく他の言語がサポートしていますが、EWS マネージ API で使用できるサンプル コードのほとんどは C# で記述されています。
  
## <a name="development-environment-for-ews"></a>EWS の開発環境
<a name="bk_EWS"> </a>

EWS を使用して、2 通りの方法でアプリケーションを開発できます。EWS を使用する最も簡単な方法は、XML 要求を含むテキスト ファイルを作成し、Exchange に送信する方法です。これを行うには、次のものが必要になります。  
  
- XML 要求を編集するためのメモ帳などの単純なテキスト エディター。任意のテキスト エディターが使用できますが、XMetal のような XML 構文の検証に役立つテキスト エディターを使用すると良いでしょう。
    
- Exchange と通信するために、SOAP XML の要求と応答を送受信できるツールまたはアプリケーション。
    
生の XML を使用する場合は、XML 形式の基本も理解しておくと役立ちます。
  
EWS を使用する 2 番目の方法は、自動生成されるプロキシを作成して、C# などの .NET 言語を使用した操作で作業できるようにする方法です。自動生成されるプロキシで操作するために必要なのものは次の通りです。
  
- プロキシ参照を作成するための Visual Studio 2005 以降のいずれかのバージョンの Visual Studio。 [無料版](https://visualstudio.microsoft.com/)をダウンロードできます。
    
- .NET Framework 2.0 以降のいずれかのバージョンの .NET Framework。 .NET Framework 3.5 は、[Microsoft ダウンロード センター](http://go.microsoft.com/fwlink/?LinkId=191777)からダウンロードできます。
    
自動生成されるプロキシを使用する場合は、C# プログラミングの知識がある程度必要です。
  
> [!NOTE]
> .NET Framework 開発者の場合は、EWS の開発には自動生成されるプロキシではなく、EWS マネージ API を使用することをお勧めします。 EWS マネージ API のオブジェクト モデルの方が自動生成されるプロキシ オブジェクト モデルよりも使いやすくなっています。 また、EWS マネージ API には[自動検出](autodiscover-for-exchange.md)が実装され、クライアント側のロジックも含まれています。 
  
## <a name="see-also"></a>関連項目

- [Exchange アプリケーションの開発環境をセットアップする](setting-up-your-exchange-application-development-environment.md)   
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)  
- [Exchange で EWS へのアクセスを制御する](how-to-control-access-to-ews-in-exchange.md)  
- [Exchange 用に EWS で生成されたオブジェクト モデル](https://msdn.microsoft.com/ja-JP/library/jj190899)
    

