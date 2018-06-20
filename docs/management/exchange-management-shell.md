---
title: Exchange 管理シェル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8cc0c4fa-9e13-45cb-88da-0486f2ac1bd0
description: Exchange 管理シェルを使用して Exchange サーバー管理用のツールを開発する方法について説明します。
ms.openlocfilehash: 1cb0328bdb0eebda0ce4eda929e1bfb21be451f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759196"
---
# <a name="exchange-management-shell"></a>Exchange 管理シェル

Exchange 管理シェルを使用して Exchange サーバー管理用のツールを開発する方法について説明します。
  
**に適用されます:** オンライン交換 |Exchange Server 2013年 |Office 365
  
Exchange 管理シェルでは、Exchange 2013 で始まるコマンドは、Exchange のオンライン、Office 365 の一部として Exchange のオンラインまたは、設置型バージョンの Exchange を管理するため、Windows PowerShell のプラットフォームをベースに豊富なセットを提供します。 Exchange 管理シェルを使用するには 2 種類のツールを作成する: コマンド ライン スクリプトが、Windows PowerShell の環境内で動作し、Exchange 管理シェル コマンドレットを使用して、マネージ インターフェイスを使用するツールです。 マネージ アプリケーションを使用すると、Exchange サーバーを管理するのにには、標準の Windows または web ベースの UI を作成します。 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a>Exchange 管理シェルについて知っておくべき事項

|についてわからない場合|説明|
|:-----|:-----|
|可用性  <br/> |Exchange 管理シェル コマンドは、Exchange が Exchange 2007 以降のバージョンを実行しているすべてのサーバーにインストールされます。<br/>クライアント アプリケーションは、Windows PowerShell 2.0 を実行しているすべてのコンピューターに展開できます。<br/> シェルへのアクセス方法の詳細については、 [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)を参照してください。  <br/> |
|言語とツール  <br/> |任意のテキスト エディターでは、Exchange 管理シェル スクリプトを作成できます。<br/>Exchange 管理シェルで使用できる Windows PowerShell スクリプトを作成するためには、多くのサード パーティ製ツールのいずれかを使用できます。  <br/> [Exchange 管理シェル オブジェクト モデル](exchange-management-shell-namespaces.md)は、.NET Framework に基づいています。<br/>Exchange 管理シェル アプリケーションを開発するのに任意の .NET 言語を使用することができます。  <br/> |
|利用可能なテスト ツールとデバッグ ツール  <br/> |Exchange 管理シェル スクリプトをテストしてデバッグするには、多くのサード パーティ製アプリケーションのいずれかを使用できます。  <br/> 管理対象の Exchange 管理シェルのアプリケーションをテストしてデバッグするには、Visual Studio とサードパーティ製のツールを使用できます。  <br/> |
|サーバー プラットフォームの要件  <br/> |Windows PowerShell 2.0 がインストールされているすべての Exchange サーバーで、Exchange 管理シェルを使用できます。  <br/> |
|クライアント プラットフォームの要件  <br/> |Exchange 管理シェルのクライアント アプリケーションでは、Windows PowerShell 2.0 が必要です。  <br/> |
|アクセス許可  <br/> |Exchange 管理シェルを実行しているアプリケーションは、ユーザーがある Exchange ストアの役割に基づくアクセス制御に影響を受けるデータ必要です。<br/>役割ベースのアクセス制御の詳細については、[役割ベースのアクセス制御と](http://technet.microsoft.com/en-us/library/dd298183.aspx)を参照してください。  <br/> |
   
このセクションの記事では、Exchange 管理ツールを作成するための重要な Exchange 管理シェルの機能について説明します。 Exchange の管理、計画、構成、または詳細については、 [Exchange](https://docs.microsoft.com/en-us/exchange/)サイトを参照してください。
  
## <a name="in-this-section"></a>このセクションの内容

- [Exchange 管理シェルのツールを作成します。](create-exchange-management-shell-tools.md)
    
- [Exchange 管理シェルの名前空間](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a>関連項目
  
- [Windows PowerShell マニュアル](https://docs.microsoft.com/en-us/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [PowerShell のスクリプト](https://docs.microsoft.com/en-us/powershell/scripting/powershell-scripting?view=powershell-6)
    

