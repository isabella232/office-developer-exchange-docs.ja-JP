---
title: 偽装を構成する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: efcef39f-e26d-4eed-95ac-36a5bf8c089f
description: Exchange 管理シェルを使用して、サービス アカウントに偽装の役割を付与する方法について説明します。
ms.openlocfilehash: 57ccef48a7553bcc06e3b3ae940b376b8555ef84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758933"
---
# <a name="configure-impersonation"></a>偽装を構成する

Exchange 管理シェルを使用して、サービス アカウントに偽装の役割を付与する方法について説明します。 
  
偽装により、サービス アプリケーションなどの呼び出し元がユーザー アカウントを偽装できるようにようなります。呼び出し元は、その呼び出し元に関連付けられたアクセス許可ではなく、偽装したアカウントに関連付けられているアクセス許可を使用して操作を実行できます。
  
Exchange Online、Office 365 の一部としての Exchange Online、および Exchange 2013 以降の Exchange の各バージョンは、役割ベースのアクセス制御 (RBAC) を使用して、アカウントにアクセス許可を割り当てます。Exchange サーバー管理者は、他のユーザーを偽装するサービス アカウントに、**New-ManagementRoleAssignment** コマンドレットを使用して [ApplicationImpersonation](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) 役割を付与する必要があります。 
  
## <a name="configuring-the-applicationimpersonation-role"></a>ApplicationImpersonation 役割の構成

**ApplicationImpersonation** 役割を自分で、または Exchenge サーバー管理者が割り当てる際には、**New-ManagementRoleAssignment** コマンドレットに次のパラメーターを使用します。 
  
-  _Name_ &ndash; 役割の割り当てのフレンドリ名。 役割を割り当てるたびに、RBAC 役割一覧に新しいエントリが作成されます。 役割の割り当ては、[Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) コマンドレットを使用すると確認できます。 
    
-  _Role_ &ndash; 割り当てる RBAC 役割。 偽装を設定する際には、**ApplicationImpersonation** 役割を割り当てます。 
    
-  _User_ &ndash; サービス アカウント。 
    
-  _CustomRecipientScope_ &ndash; サービス アカウントが偽装できるユーザーのスコープ。 サービス アカウントは、指定されたスコープ内でのみ他のユーザーを偽装できます。 スコープが指定されていない場合、サービス アカウントには組織内のすべてのユーザーを範囲とする **ApplicationImpersonation** 役割が付与されます。 [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) コマンドレットを使用すると、カスタムの管理スコープを作成できます。 
    
偽装を構成するには、次のものが必要です。
  
- Exchange サーバーの管理者の資格情報。
    
- ドメイン管理者の資格情報。または役割とスコープの作成および割り当ての権限のある、その他の資格情報。
    
- Exchange 管理ツール。このツールは、コマンドを実行するコンピューターにインストールされています。
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a>組織内のすべてのユーザーの偽装を構成するには

1. Exchange 管理シェルを開きます。[スタート] メニューから、 **[すべてのプログラム]** > **[Microsoft Exchange Server 2013]** を選択します。 
    
2. **New-ManagementRoleAssignment** コマンドレットを実行して、指定したユーザーに偽装の権限を追加します。次の例は、サービス アカウントが組織内のその他すべてのユーザーを偽装できるようにする偽装の構成方法を示しています。 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a>特定のユーザーまたはユーザー ループの偽装を構成するには

1. Exchange 管理シェルを開きます。[スタート] メニューから、 **[すべてのプログラム]** > **[Microsoft Exchange Server 2013]** を選択します。 
    
2. **New-ManagementScope** コマンドレットを実行して、偽装の役割の割り当て先にできるスコープを作成します。既存のスコープが利用できる場合は、この手順を省略できます。次の例は、特定のグループを対象とした管理スコープの作成方法を示しています。 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   _New-ManagementScope_ コマンドレットの **RecipientRestrictionFilter** パラメーターによって、スコープのメンバーを定義します。 フィルターの作成には、**Identity** オブジェクトのプロパティを使用できます。 次の例は、ユーザー名が "john" の単一のユーザーに結果を制限するフィルターです。 
    
   ```powershell
   Name -eq "john"
   ```

3. **New-ManagementRoleAssignment** コマンドレットを実行して、指定したスコープのメンバーを偽装する権限を追加します。次の例は、スコープ内のすべてのユーザーを偽装するようにサービス アカウントを構成する方法を示しています。 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


管理者が偽装の権限を付与したら、別のユーザーのアカウントに対する呼び出しを行うためにサービス アカウントを使用できます。役割の割り当ては、[Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) コマンドレットを使用すると確認できます。 
  
## <a name="see-also"></a>関連項目

- [Exchange の偽装と EWS](impersonation-and-ews-in-exchange.md)
- [ApplicationImpersonation 役割](http://technet.microsoft.com/ja-JP/library/dd776119%28v=exchg.150%29.aspx)   
- [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

