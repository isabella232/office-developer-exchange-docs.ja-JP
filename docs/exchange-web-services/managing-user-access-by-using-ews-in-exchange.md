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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759089"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a>Exchange において EWS を使用してユーザー アクセスを管理する

Exchange サーバーに対するユーザー アカウントのアクセス権を管理するためのオプションについて説明します。
  
Exchange Web サービス (EWS) と EWS マネージ API には、Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2013 以降の Exchange バージョンでアカウントを管理するために使用できるいくつかの操作があります。 次の図に示されているこれらの操作を使用すると、デリゲートを管理して、他のアカウントのフォルダー アクセス許可を設定できます。 
  
**デリゲートおよびフォルダー アクセスのための EWS 操作**

![EWS ユーザー管理オプション](media/Exchange_ManagingUserAccess_1.png)
  
アプリケーションで、Exchange サーバーにおけるアカウントの制御をさらに必要とする場合は、Exchange 管理シェル コマンドレットを使用してアカウントを管理できます。Exchange 管理シェル コマンドレットは、次のいずれかの方法で呼び出すことができます。
  
- Exchange 管理シェル コマンドレットを呼び出す C# または Visual Basic を使用してアプリケーションを作成します。 [Exchange 管理シェル API ドキュメント](../management/exchange-management-shell.md)に記されているサンプル コードを調べて、コマンドレットの呼び出し方法を確認できます。 
    
- Windows PowerShell および Windows PowerShell スクリプトを使用して、Exchange 管理シェル コマンドレットを呼び出します。 
  [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) のすべての一覧が、使用法を示す例と共に記載されています。 
    
## <a name="see-also"></a>関連項目

- [EWS アプリケーションの設定](setting-up-your-ews-application.md)   
- 
  [Exchange 2013 コマンドレット](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)  
    

