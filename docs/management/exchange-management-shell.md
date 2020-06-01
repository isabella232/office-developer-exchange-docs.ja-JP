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
ms.openlocfilehash: 38e75339a4ad97cf8ff99e1cbe9c01059e157941
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44435808"
---
# <a name="exchange-management-shell"></a>Exchange 管理シェル

Exchange 管理シェルを使用して Exchange サーバー管理用のツールを開発する方法について説明します。
  
**適用対象:** Exchange Online |Exchange Server 2013 |Office 365
  
Exchange 管理シェルは、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2013 以降のオンプレミス バージョンの Exchange を管理するため、Windows PowerShell のプラットフォームをベースにした豊富なコマンド セットを提供します。 Exchange 管理シェルを使用すると、Windows PowerShell 環境内で動作するコマンドラインスクリプトと、管理インターフェイスを使用して Exchange 管理シェルコマンドレットを使用するツールという2種類のツールを作成できます。 管理されたアプリケーションを使用して、Exchange サーバーを管理するための標準の Windows または web ベースの UI を作成できます。 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a>Exchange 管理シェルについて知っておくべき事項

|ご参考までに|説明|
|:-----|:-----|
|Availability  <br/> |Exchange 管理シェル コマンドは、Exchange 2007 以降のバージョンの Exchange を実行しているすべてのサーバーにインストールされます。<br/>クライアント アプリケーションは、Windows PowerShell 2.0 を実行しているすべてのコンピューターに展開できます。<br/> シェルへのアクセスについては、「 [Exchange Server PowerShell (Exchange Management shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)」を参照してください。  <br/> |
|言語とツール  <br/> |Exchange 管理シェル スクリプトは任意のテキスト エディターで作成できます。<br/>Exchange 管理シェルで使用できる Windows PowerShell スクリプトを作成するために、多くのサード パーティ製ツールのいずれかを使用できます。  <br/> [Exchange 管理シェルのオブジェクト モデル](exchange-management-shell-namespaces.md)は、.NET Framework に基づいています。<br/>Exchange 管理シェル アプリケーションを開発するために任意の .NET 言語を使用することができます。  <br/> |
|利用可能なテスト ツールとデバッグ ツール  <br/> |Exchange 管理シェル スクリプトをテストしてデバッグするには、多くのサード パーティ製アプリケーションのいずれかを使用できます。  <br/> 管理対象の Exchange 管理シェルのアプリケーションをテストしてデバッグするには、Visual Studio とサードパーティ製のツールを使用できます。  <br/> |
|サーバー プラットフォームの要件  <br/> |Windows PowerShell 2.0 がインストールされているすべての Exchange サーバーで、Exchange 管理シェルを使用できます。  <br/> |
|クライアント プラットフォームの要件  <br/> |Exchange 管理シェルのクライアント アプリケーションでは、Windows PowerShell 2.0 が必要です。  <br/> |
|アクセス許可  <br/> |Exchange 管理シェル アプリケーションを実行するには、ユーザーが Exchange ストアの影響を受けるデータに対する役割ベースのアクセス制御の権限が必要です。<br/>役割ベースのアクセス制御の詳細については、「[役割ベース](https://technet.microsoft.com/library/dd298183.aspx)のアクセス制御について」を参照してください。  <br/> |
   
このセクションの記事では、Exchange 管理ツールを作成するための重要な Exchange 管理シェルの機能について説明します。 Exchange の計画、構成、または保守の詳細については、「 [exchange](https://docs.microsoft.com/exchange/)サイト」を参照してください。
  
## <a name="in-this-section"></a>このセクションの内容

- [Exchange 管理シェル ツールの作成](create-exchange-management-shell-tools.md)
    
- [Exchange 管理シェルの名前空間](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a>関連項目
  
- [Windows PowerShell ドキュメント](https://docs.microsoft.com/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [PowerShell スクリプト](https://docs.microsoft.com/powershell/scripting/powershell-scripting?view=powershell-6)
    

