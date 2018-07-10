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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758933"
---
# <a name="configure-impersonation"></a><span data-ttu-id="19f63-103">偽装を構成します。</span><span class="sxs-lookup"><span data-stu-id="19f63-103">Configure impersonation</span></span>

<span data-ttu-id="19f63-104">Exchange 管理シェルを使用して、サービス アカウントに偽装の役割を付与する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="19f63-104">Learn how to grant the impersonation role to a service account by using the Exchange Management Shell.</span></span> 
  
<span data-ttu-id="19f63-p101">偽装により、サービス アプリケーションなどの呼び出し元がユーザー アカウントを偽装できるようにようなります。呼び出し元は、その呼び出し元に関連付けられたアクセス許可ではなく、偽装したアカウントに関連付けられているアクセス許可を使用して操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="19f63-p101">Impersonation enables a caller, such as a service application, to impersonate a user account. The caller can perform operations by using the permissions that are associated with the impersonated account instead of the permissions associated with the caller's account.</span></span>
  
<span data-ttu-id="19f63-p102">Exchange Online、Office 365 の一部としての Exchange Online、および Exchange 2013 以降の Exchange の各バージョンは、役割ベースのアクセス制御 (RBAC) を使用して、アカウントにアクセス許可を割り当てます。Exchange サーバー管理者は、他のユーザーを偽装するサービス アカウントに、**New-ManagementRoleAssignment** コマンドレットを使用して [ApplicationImpersonation](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) 役割を付与する必要があります。</span><span class="sxs-lookup"><span data-stu-id="19f63-p102">Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013 use role-based access control (RBAC) to assign permissions to accounts. Your Exchange server administrator will need to grant any service account that will be impersonating other users the **ApplicationImpersonation** role by using the [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) cmdlet.</span></span> 
  
## <a name="configuring-the-applicationimpersonation-role"></a><span data-ttu-id="19f63-109">ApplicationImpersonation 役割の構成</span><span class="sxs-lookup"><span data-stu-id="19f63-109">Configuring the ApplicationImpersonation role</span></span>

<span data-ttu-id="19f63-110">Exchange サーバー管理者または自分で **ApplicationImpersonation** 役割を割り当てるときには、次のパラメーターを **New-ManagementRoleAssignment** コマンドレットに使用します。</span><span class="sxs-lookup"><span data-stu-id="19f63-110">When you or your Exchanger server administrator assigns the **ApplicationImpersonation** role, use the following parameters of the **New-ManagementRoleAssignment** cmdlet:</span></span> 
  
-  <span data-ttu-id="19f63-111">_名_&ndash;ロールの割り当ての表示名です。</span><span class="sxs-lookup"><span data-stu-id="19f63-111">_Name_ &ndash; The friendly name of the role assignment.</span></span> <span data-ttu-id="19f63-112">役割を割り当てるたびに、RBAC 役割一覧に新しいエントリが作成されます。</span><span class="sxs-lookup"><span data-stu-id="19f63-112">Each time that you assign a role, an entry is made in the RBAC roles list.</span></span> <span data-ttu-id="19f63-113">役割の割り当ては、 [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) コマンドレットを使用して確認できます。</span><span class="sxs-lookup"><span data-stu-id="19f63-113">You can verify role assignments by using the [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
    
-  <span data-ttu-id="19f63-114">_ロール_&ndash;の RBAC の役割を割り当てる。</span><span class="sxs-lookup"><span data-stu-id="19f63-114">_Role_ &ndash; The RBAC role to assign.</span></span> <span data-ttu-id="19f63-115">偽装を設定するときには、 **ApplicationImpersonation** 役割を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="19f63-115">When you set up impersonation, you assign the **ApplicationImpersonation** role.</span></span> 
    
-  <span data-ttu-id="19f63-116">_ユーザー_&ndash;サービス アカウントです。</span><span class="sxs-lookup"><span data-stu-id="19f63-116">_User_ &ndash; The service account.</span></span> 
    
-  <span data-ttu-id="19f63-117">_CustomRecipientScope_&ndash;サービス アカウントを偽装するユーザーのスコープです。</span><span class="sxs-lookup"><span data-stu-id="19f63-117">_CustomRecipientScope_ &ndash; The scope of users that the service account can impersonate.</span></span> <span data-ttu-id="19f63-118">サービス アカウントは、指定されたスコープ内でのみ他のユーザーを偽装できます。</span><span class="sxs-lookup"><span data-stu-id="19f63-118">The service account will only be allowed to impersonate other users within the specified scope.</span></span> <span data-ttu-id="19f63-119">スコープが指定されていない場合、サービス アカウントには組織内のすべてのユーザーを範囲とする **ApplicationImpersonation** 役割が付与されます。</span><span class="sxs-lookup"><span data-stu-id="19f63-119">If no scope is specified, the service account is granted the **ApplicationImpersonation** role over all users in an organization.</span></span> <span data-ttu-id="19f63-120">[New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) コマンドレットを使用すると、カスタムの管理スコープを作成できます。</span><span class="sxs-lookup"><span data-stu-id="19f63-120">You can create custom management scopes by using the [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) cmdlet.</span></span> 
    
<span data-ttu-id="19f63-121">偽装を構成するには、次のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="19f63-121">Before you can configure impersonation, you need:</span></span>
  
- <span data-ttu-id="19f63-122">Exchange サーバーの管理者の資格情報。</span><span class="sxs-lookup"><span data-stu-id="19f63-122">Administrative credentials for the Exchange server.</span></span>
    
- <span data-ttu-id="19f63-123">ドメイン管理者の資格情報。または役割とスコープの作成および割り当ての権限のある、その他の資格情報。</span><span class="sxs-lookup"><span data-stu-id="19f63-123">Domain Administrator credentials, or other credentials with the permission to create and assign roles and scopes.</span></span>
    
- <span data-ttu-id="19f63-p106">Exchange 管理ツール。このツールは、コマンドを実行するコンピューターにインストールされています。</span><span class="sxs-lookup"><span data-stu-id="19f63-p106">Exchange management tools. These are installed on the computer from which you will run the commands.</span></span>
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a><span data-ttu-id="19f63-126">組織内のすべてのユーザーの偽装を構成するには</span><span class="sxs-lookup"><span data-stu-id="19f63-126">To configure impersonation for all users in an organization</span></span>

1. <span data-ttu-id="19f63-p107">Exchange 管理シェルを開きます。[スタート] メニューから、 **[すべてのプログラム]** > **[Microsoft Exchange Server 2013]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="19f63-p107">Open the Exchange Management Shell. From the Start menu, choose **All Programs** > **Microsoft Exchange Server 2013**.</span></span> 
    
2. <span data-ttu-id="19f63-p108">**New-ManagementRoleAssignment** コマンドレットを実行して、指定したユーザーに偽装の権限を追加します。次の例は、サービス アカウントが組織内のその他すべてのユーザーを偽装できるようにする偽装の構成方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="19f63-p108">Run the **New-ManagementRoleAssignment** cmdlet to add the impersonation permission to the specified user. The following example shows how to configure impersonation to enable a service account to impersonate all other users in an organization.</span></span> 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a><span data-ttu-id="19f63-131">特定のユーザーまたはユーザー ループの偽装を構成するには</span><span class="sxs-lookup"><span data-stu-id="19f63-131">To configure impersonation for specific users or groups of users</span></span>

1. <span data-ttu-id="19f63-p109">Exchange 管理シェルを開きます。[スタート] メニューから、 **[すべてのプログラム]** > **[Microsoft Exchange Server 2013]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="19f63-p109">Open the Exchange Management Shell. From the Start menu, choose **All Programs** > **Microsoft Exchange Server 2013**.</span></span> 
    
2. <span data-ttu-id="19f63-p110">**New-ManagementScope** コマンドレットを実行して、偽装の役割の割り当て先にできるスコープを作成します。既存のスコープが利用できる場合は、この手順を省略できます。次の例は、特定のグループを対象とした管理スコープの作成方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="19f63-p110">Run the **New-ManagementScope** cmdlet to create a scope to which the impersonation role can be assigned. If an existing scope is available, you can skip this step. The following example shows how to create a management scope for a specific group.</span></span> 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   <span data-ttu-id="19f63-137">**新規 ManagementScope**コマンドレットの_RecipientRestrictionFilter_パラメーターでは、スコープのメンバーを定義します。</span><span class="sxs-lookup"><span data-stu-id="19f63-137">The _RecipientRestrictionFilter_ parameter of the **New-ManagementScope** cmdlet defines the members of the scope.</span></span> <span data-ttu-id="19f63-138">フィルターの作成には、 **Identity** オブジェクトのプロパティを使用できます。</span><span class="sxs-lookup"><span data-stu-id="19f63-138">You can use the properties of the **Identity** object to create the filter.</span></span> <span data-ttu-id="19f63-139">次の例は、ユーザー名が "john" の単一のユーザーに結果を制限するフィルターです。</span><span class="sxs-lookup"><span data-stu-id="19f63-139">The following example is a filter that restricts the result to a single user with the user name "john."</span></span> 
    
   ```powershell
   Name -eq "john"
   ```

3. <span data-ttu-id="19f63-p112">**New-ManagementRoleAssignment** コマンドレットを実行して、指定したスコープのメンバーを偽装する権限を追加します。次の例は、スコープ内のすべてのユーザーを偽装するようにサービス アカウントを構成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="19f63-p112">Run the **New-ManagementRoleAssignment** cmdlet to add the permission to impersonate the members of the specified scope. The following example shows how to configure a service account to impersonate all users in a scope.</span></span> 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


<span data-ttu-id="19f63-p113">管理者が偽装の権限を付与したら、別のユーザーのアカウントに対する呼び出しを行うためにサービス アカウントを使用できます。役割の割り当ては、[Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) コマンドレットを使用すると確認できます。</span><span class="sxs-lookup"><span data-stu-id="19f63-p113">After your administrator grants impersonation permissions, you can use the service account to make calls against other users' accounts. You can verify role assignments by using the [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="19f63-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="19f63-144">See also</span></span>

- [<span data-ttu-id="19f63-145">Exchange の偽装と EWS</span><span class="sxs-lookup"><span data-stu-id="19f63-145">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
- [<span data-ttu-id="19f63-146">ApplicationImpersonation 役割</span><span class="sxs-lookup"><span data-stu-id="19f63-146">ApplicationImpersonation role</span></span>](http://technet.microsoft.com/ja-jp/library/dd776119%28v=exchg.150%29.aspx)   
- [<span data-ttu-id="19f63-147">新しい-ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="19f63-147">New-ManagementRoleAssignment</span></span>](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [<span data-ttu-id="19f63-148">Get ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="19f63-148">Get-ManagementRoleAssignment</span></span>](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

