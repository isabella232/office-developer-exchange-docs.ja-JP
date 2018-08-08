---
title: Exchange での EWS に対するアクセスの制御
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: ユーザー、アプリケーション、組織全体の EWS へのアクセスを制御する方法を確認します。
ms.openlocfilehash: 956c28faba105ecf2a6b1452abe629ea2fc930e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758928"
---
# <a name="control-access-to-ews-in-exchange"></a>Exchange での EWS に対するアクセスの制御

ユーザー、アプリケーション、組織全体の EWS へのアクセスを制御する方法を確認します。
  
アプリケーション内で EWS マネージ API を使用しているにせよ EWS を直接使用しているにせよ、Exchange Web サービス (EWS) へのアクセスを制御できます。Exchange サーバーへの管理者アクセス権があれば、グローバルにアクセス制御するための Exchange Management Shell を使用して、ユーザーごとおよびアプリケーションごとに、EWS へのアクセスを管理できます。
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a>アクセス制御を構成するための Exchange 管理シェル コマンドレット
<a name="bk_Cmdlets"> </a>

次の Exchange 管理シェル コマンドレットを使用して、現在のアクセス構成を表示し、EWS のアクセス制御を設定できます。
  
- [Get-CASMailbox](http://technet.microsoft.com/ja-JP/library/bb124754.aspx) - 特定のメールボックスに対して設定されているパラメーターを表示します。   
- [Set-CASMailbox](http://technet.microsoft.com/ja-JP/library/bb125264.aspx) - 特定のメールボックスのパラメーターを設定します。    
- [Get-OrganizationConfig](http://technet.microsoft.com/ja-JP/library/aa997571.aspx) - 組織全体のパラメーターを表示します。    
- [Set-OrganizationConfig](http://technet.microsoft.com/ja-JP/library/aa997443.aspx) - 組織全体のパラメーターを設定します。 

<a name="bk_Examples"> </a>

## <a name="examples-controlling-access-to-ews"></a>例: EWS へのアクセスを制御する

アプリケーションへのアクセスを制御する方法を説明するいくつかのシナリオを見てみましょう。
  
**表 1. EWS へのアクセスを制御するためのコマンド**

|目的 |使用するコマンド|
|:-----|:-----|
|EWS を使用しないよう、すべてのクライアント アプリケーションをブロックする。 | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/>これは、AllowList に記載されているアプリケーションの接続を許可します。この例では、AllowList にアプリケーションが含まれていないため、EWS を使用できるアプリケーションはありません。 |
|リストに載っているクライアント アプリケーションに EWS の使用を許可する。 | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/>これは、特定のアプリケーションに対して EWS の使用を許可します。 この例では、"OWA/" から始まるユーザー エージェント文字列を含むすべてのアプリケーションにアクセスが許可されます。 |
|明示的にブロックされているものを除き、すべてのクライアント アプリケーションに EWS の使用を許可する。 | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/>この例では、"OWA/" で始まるユーザー エージェント文字列を含むアプリケーションのみをブロックして EWS を使用できないようにします。 |
|すべてのクライアント アプリケーションに EWS の使用を許可する。 | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> ブロック リストが指定されていないため、すべてのアプリケーションが EWS を使用できます。 |
|EWS を使用できないよう、組織全体をブロックする。 | `Set-OrganizationConfig -EwsEnabled:$false` |
|EWS を使用できるよう、組織全体を許可する。 | `Set-OrganizationConfig -EwsEnabled:$true`|
|EWS を使用できないよう、個々のメールボックスをブロックする。 | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|個々のメールボックスに EWS の使用を許可する。 | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a>関連項目

- [EWS アプリケーションの設定](setting-up-your-ews-application.md)    
- [Exchange で EWS へのクライアント アプリケーションのアクセスを制御する](controlling-client-application-access-to-ews-in-exchange.md)   
- 
  [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [Windows PowerShell](http://msdn.microsoft.com/ja-JP/library/dd835506%28v=vs.85%29.aspx)
    

