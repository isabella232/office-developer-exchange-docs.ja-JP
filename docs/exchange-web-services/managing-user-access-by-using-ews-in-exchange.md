---
title: Exchange において EWS を使用してユーザー アクセスを管理する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Exchange サーバーに対するユーザー アカウントのアクセス権を管理するためのオプションについて説明します。
ms.openlocfilehash: d93f521f08f93b44b4ecc1f258b03ed24ebdd3dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759089"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a>Exchange において EWS を使用してユーザー アクセスを管理する

Exchange サーバーに対するユーザー アカウントのアクセス権を管理するためのオプションについて説明します。
  
Exchange Web サービス (EWS) と、EWS のマネージ API Exchange Online、Office 365 の一部として Exchange のオンラインまたは Exchange 2013 で開始する Exchange のバージョンのアカウントを管理するために使用できる操作の数に制限を提供します。 委任を管理して、他のアカウントのフォルダーのアクセス許可を設定するのには、次の図に示すように操作を使用できます。 
  
**デリゲートおよびフォルダーのアクセスの EWS の操作**

![EWS ユーザー管理オプション](media/Exchange_ManagingUserAccess_1.png)
  
アプリケーションで、Exchange サーバーにおけるアカウントの制御をさらに必要とする場合は、Exchange 管理シェル コマンドレットを使用してアカウントを管理できます。Exchange 管理シェル コマンドレットは、次のいずれかの方法で呼び出すことができます。
  
- C# または Exchange 管理シェル コマンドレットを呼び出す Visual Basic を使用してアプリケーションを作成します。 コマンドレットを呼び出す方法については、 [Exchange 管理シェルの API ドキュメント](../management/exchange-management-shell.md)のサンプル コードを見ることができます。 
    
- Exchange 管理シェル コマンドレットを呼び出す Windows PowerShell および Windows PowerShell スクリプトを使用します。 [PowerShell の Exchange Server (Exchange 管理シェル)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)を使用する方法を示す例との完全な一覧が表示されます。 
    
## <a name="see-also"></a>関連項目

- [EWS アプリケーションを設定します。](setting-up-your-ews-application.md)   
- [Exchange 2013 コマンドレット](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)  
    

