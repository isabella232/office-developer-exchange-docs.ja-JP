---
title: 偽装を構成します。
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: efcef39f-e26d-4eed-95ac-36a5bf8c089f
description: Exchange 管理シェルを使用して、サービス アカウントに偽装の役割を付与する方法について説明します。
ms.openlocfilehash: 57ccef48a7553bcc06e3b3ae940b376b8555ef84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758933"
---
# <a name="configure-impersonation"></a>偽装を構成します。

Exchange 管理シェルを使用して、サービス アカウントに偽装の役割を付与する方法について説明します。 
  
偽装により、サービス アプリケーションなどの呼び出し元がユーザー アカウントを偽装できるようにようなります。呼び出し元は、その呼び出し元に関連付けられたアクセス許可ではなく、偽装したアカウントに関連付けられているアクセス許可を使用して操作を実行できます。
  
Exchange Online、Office 365 の一部としての Exchange Online、および Exchange 2013 以降の Exchange の各バージョンは、役割ベースのアクセス制御 (RBAC) を使用して、アカウントにアクセス許可を割り当てます。Exchange サーバー管理者は、他のユーザーを偽装するサービス アカウントに、**New-ManagementRoleAssignment** コマンドレットを使用して [ApplicationImpersonation](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) 役割を付与する必要があります。 
  
## <a name="configuring-the-applicationimpersonation-role"></a>ApplicationImpersonation 役割の構成

Exchange サーバー管理者または自分で **ApplicationImpersonation** 役割を割り当てるときには、次のパラメーターを **New-ManagementRoleAssignment** コマンドレットに使用します。 
  
-  _名_&ndash;ロールの割り当ての表示名です。 役割を割り当てるたびに、RBAC 役割一覧に新しいエントリが作成されます。 役割の割り当ては、 [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) コマンドレットを使用して確認できます。 
    
-  _ロール_&ndash;の RBAC の役割を割り当てる。 偽装を設定するときには、 **ApplicationImpersonation** 役割を割り当てます。 
    
-  _ユーザー_&ndash;サービス アカウントです。 
    
-  _CustomRecipientScope_&ndash;サービス アカウントを偽装するユーザーのスコープです。 サービス アカウントは、指定されたスコープ内でのみ他のユーザーを偽装できます。 スコープが指定されていない場合、サービス アカウントには組織内のすべてのユーザーを範囲とする **ApplicationImpersonation** 役割が付与されます。 [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) コマンドレットを使用すると、カスタムの管理スコープを作成できます。 
    
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

   **新規 ManagementScope**コマンドレットの_RecipientRestrictionFilter_パラメーターでは、スコープのメンバーを定義します。 フィルターの作成には、 **Identity** オブジェクトのプロパティを使用できます。 次の例は、ユーザー名が "john" の単一のユーザーに結果を制限するフィルターです。 
    
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
- [ApplicationImpersonation 役割](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)   
- [新しい-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [Get ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

