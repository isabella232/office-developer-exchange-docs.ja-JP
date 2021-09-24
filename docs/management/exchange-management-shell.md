---
title: Exchange 管理シェル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8cc0c4fa-9e13-45cb-88da-0486f2ac1bd0
description: Exchange 管理シェルを使用して Exchange サーバー管理用のツールを開発する方法について説明します。
ms.openlocfilehash: ee1cbcb174c7153ca6cd9bb089580b372bf9029b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516154"
---
# <a name="exchange-management-shell"></a>Exchange 管理シェル

Exchange 管理シェルを使用して Exchange サーバー管理用のツールを開発する方法について説明します。
  
**適用対象: Exchange Online |** Exchange Server 2013 |Office 365
  
Exchange 管理シェルは、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2013 以降のオンプレミス バージョンの Exchange を管理するため、Windows PowerShell のプラットフォームをベースにした豊富なコマンド セットを提供します。Exchange 管理シェルを使用して 2 種類のツールを作成できます。Windows PowerShell の環境内で動作するコマンド ライン スクリプトと、マネージ インターフェイスで Exchange 管理シェル コマンドレットを使用するツールです。マネージ アプリケーションを使用すると、Exchange サーバーを管理するための標準 Windows UI か Web ベースの UI を作成できます。  
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a>Exchange 管理シェルについて知っておくべき事項

|について疑問に思っている場合|説明|
|:-----|:-----|
|可用性  <br/> |Exchange 管理シェル コマンドは、Exchange 2007 以降のバージョンの Exchange を実行しているすべてのサーバーにインストールされます。<br/>クライアント アプリケーションは、Windows PowerShell 2.0 を実行しているすべてのコンピューターに展開できます。<br/> シェルへのアクセスの詳細については[、「powerShell (Exchange Server管理シェルExchangeを参照してください](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)。  <br/> |
|言語とツール  <br/> |Exchange 管理シェル スクリプトは任意のテキスト エディターで作成できます。<br/>Exchange 管理シェルで使用できる Windows PowerShell スクリプトを作成するために、多くのサード パーティ製ツールのいずれかを使用できます。  <br/> [Exchange 管理シェルのオブジェクト モデル](exchange-management-shell-namespaces.md)は、.NET Framework に基づいています。<br/>Exchange 管理シェル アプリケーションを開発するために任意の .NET 言語を使用することができます。  <br/> |
|利用可能なテスト ツールとデバッグ ツール  <br/> |Exchange 管理シェル スクリプトをテストしてデバッグするには、多くのサード パーティ製アプリケーションのいずれかを使用できます。  <br/> 管理対象の Exchange 管理シェルのアプリケーションをテストしてデバッグするには、Visual Studio とサードパーティ製のツールを使用できます。  <br/> |
|サーバー プラットフォームの要件  <br/> |Windows PowerShell 2.0 がインストールされているすべての Exchange サーバーで、Exchange 管理シェルを使用できます。  <br/> |
|クライアント プラットフォームの要件  <br/> |Exchange 管理シェルのクライアント アプリケーションでは、Windows PowerShell 2.0 が必要です。  <br/> |
|アクセス許可  <br/> |Exchange 管理シェル アプリケーションを実行するには、ユーザーが Exchange ストアの影響を受けるデータに対する役割ベースのアクセス制御の権限が必要です。<br/>役割ベースのアクセス制御の詳細については、「役割ベースのアクセス制御 [について」を参照してください](https://technet.microsoft.com/library/dd298183.aspx)。  <br/> |
   
このセクションの記事では、Exchange 管理ツールを作成するための重要な Exchange 管理シェルの機能について説明します。 計画、構成、または保守の詳細については、「Exchange」を[Exchange](https://docs.microsoft.com/exchange/)してください。
  
## <a name="in-this-section"></a>このセクションの内容

- [Exchange 管理シェル ツールの作成](create-exchange-management-shell-tools.md)
    
- [Exchange 管理シェルの名前空間](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a>関連項目
  
- [Windows PowerShellドキュメント](https://docs.microsoft.com/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [PowerShell スクリプト](https://docs.microsoft.com/powershell/scripting/powershell-scripting?view=powershell-6)
    

