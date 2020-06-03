---
title: Exchange 管理シェルを使用してメールユーザーの一覧を取得する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.assetid: 8b790dc8-5c4f-4acf-bbe7-63523395fbe7
description: Exchange 管理シェル コマンドレットを使用して、Exchange メールボックスのユーザーの一覧を取得するツールを作成する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: 817d92ef1bb88017f471681b448c052ecaa54e7e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44435710"
---
# <a name="get-a-list-of-mail-users-by-using-the-exchange-management-shell"></a><span data-ttu-id="e83d7-103">Exchange 管理シェルを使用してメールユーザーの一覧を取得する</span><span class="sxs-lookup"><span data-stu-id="e83d7-103">Get a list of mail users by using the Exchange Management Shell</span></span>

<span data-ttu-id="e83d7-104">Exchange 管理シェル コマンドレットを使用して、Exchange メールボックスのユーザーの一覧を取得するツールを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-104">Learn how to use Exchange Management Shell cmdlets to create a tool that returns a list of Exchange mailbox users.</span></span>
  
<span data-ttu-id="e83d7-105">**適用対象:** Exchange Online |Exchange Server 2013 |Office 365</span><span class="sxs-lookup"><span data-stu-id="e83d7-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span> 
  
<span data-ttu-id="e83d7-106">Exchange 管理シェル コマンドレットを呼び出す管理ツールを使用して、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2013 以降のバージョンの Exchange からユーザーの一覧を取得することは、2 段階のプロセスです。</span><span class="sxs-lookup"><span data-stu-id="e83d7-106">Getting a list of users from Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013 by using a managed tool that calls an Exchange Management Shell cmdlet is a two-step process.</span></span> <span data-ttu-id="e83d7-107">最初に、Exchange サーバー上のリモートの実行空間を確立し、次にリモートの実行空間内でユーザー情報を取得するコマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-107">First, you establish a remote runspace on an Exchange server; then, you run the cmdlet to retrieve the user information in the remote runspace.</span></span> 

<span data-ttu-id="e83d7-108">リモートの実行空間に接続するには、組織のセキュリティ要件を満たしている認証スキームを使用して、Exchange サーバーとの認証を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="e83d7-108">To connect to the remote runspace, you have to authenticate with the Exchange server by using the authentication scheme that meets the security requirements of your organization.</span></span> 

<span data-ttu-id="e83d7-109">この記事では、リモートの実行空間を設定し、Exchange サーバーからユーザーの一覧を取得するための Exchange 管理シェル コマンドレットを実行するのに使用できるコード例を提供します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-109">This article provides code examples that you can use to set up a remote runspace and run an Exchange Management Shell cmdlet to get a list of users from an Exchange server.</span></span>

<span data-ttu-id="e83d7-110"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="e83d7-110"><a name="bk_prerequisites"> </a></span></span>

## <a name="prerequisites-for-getting-a-list-of-mailbox-users"></a><span data-ttu-id="e83d7-111">メールボックスのユーザーの一覧を取得するための前提条件</span><span class="sxs-lookup"><span data-stu-id="e83d7-111">Prerequisites for getting a list of mailbox users</span></span>

<span data-ttu-id="e83d7-112">このタスクを実行するには、次の名前空間への参照が必要です。</span><span class="sxs-lookup"><span data-stu-id="e83d7-112">To perform this task, you need a reference to the following namespaces:</span></span>
  
- <span data-ttu-id="e83d7-113">**System.web モデル**</span><span class="sxs-lookup"><span data-stu-id="e83d7-113">**System.Collections.ObjectModel**</span></span>
- <span data-ttu-id="e83d7-114">**システム管理**</span><span class="sxs-lookup"><span data-stu-id="e83d7-114">**System.Management.Automation**</span></span>
- <span data-ttu-id="e83d7-115">**システムの管理**</span><span class="sxs-lookup"><span data-stu-id="e83d7-115">**System.Management.Automation.Remoting**</span></span>
- <span data-ttu-id="e83d7-116">**システム管理の自動化**</span><span class="sxs-lookup"><span data-stu-id="e83d7-116">**System.Management.Automation.Runspaces**</span></span>
    
> [!NOTE]
>  <span data-ttu-id="e83d7-p102">Visual Studio を使用してアプリケーションを作成する場合は、System.Management.Automation.dll アセンブリへの参照をプロジェクトに追加する必要があります。アセンブリは次の場所のいずれかにあります。</span><span class="sxs-lookup"><span data-stu-id="e83d7-p102">When you are using Visual Studio to create an application, you must add a reference to the System.Management.Automation.dll assembly to the project. The assembly can be found in one of the following locations:</span></span>
> - <span data-ttu-id="e83d7-119">オペレーティング システムが Windows XP および Windows Vista の場合、Windows PowerShell のインストール ディレクトリ ($PSHOME)。</span><span class="sxs-lookup"><span data-stu-id="e83d7-119">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span>
> - <span data-ttu-id="e83d7-120">オペレーティング システムが Windows 7 および Windows 8 の場合は次のフォルダー:Windows\assembly\GAC_MSIL\System.Management.Automation。</span><span class="sxs-lookup"><span data-stu-id="e83d7-120">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
<span data-ttu-id="e83d7-121">Exchange 管理シェルコマンドレットを自動化するアプリケーションを実行しているコンピューターの実行空間に、Exchange 2013 管理スナップインを読み込まないようにします。</span><span class="sxs-lookup"><span data-stu-id="e83d7-121">Do not load the Exchange 2013 Management snap-in into the runspace on computers that are running applications that automate Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="e83d7-122">代わりに、この記事で後述するように、アプリケーションはリモートの実行空間を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e83d7-122">The application should instead create a remote runspace, as described later in this article.</span></span>

<span data-ttu-id="e83d7-123"><a name="bk_gettinglistmailbox"> </a></span><span class="sxs-lookup"><span data-stu-id="e83d7-123"><a name="bk_gettinglistmailbox"> </a></span></span>

## <a name="connect-to-a-remote-runspace-on-an-exchange-server"></a><span data-ttu-id="e83d7-124">Exchange サーバーのリモートの実行空間に接続する</span><span class="sxs-lookup"><span data-stu-id="e83d7-124">Connect to a remote runspace on an Exchange server</span></span>

<span data-ttu-id="e83d7-p104">Exchange 管理シェル コマンドレットを使用するリモートの実行空間への接続に使用する方法は、使用している認証スキームによって異なります。このセクションでは、次の表に記載されている認証方法を使用している場合に、リモートの実行空間に接続する方法を示すコード例を提供します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-p104">The method that you use to connect to a remote runspace to use an Exchange Management Shell cmdlet varies based on the authentication scheme that you are using. This section provides code examples that show how to connect to a remote runspace when you are using an authentication method listed in the following table.</span></span>
  
|<span data-ttu-id="e83d7-127">**認証方法**</span><span class="sxs-lookup"><span data-stu-id="e83d7-127">**Authentication method**</span></span>|<span data-ttu-id="e83d7-128">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="e83d7-128">**Applies to**</span></span>|<span data-ttu-id="e83d7-129">**URI**</span><span class="sxs-lookup"><span data-stu-id="e83d7-129">**URI**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="e83d7-130">基本認証を使用して Exchange Online のリモートの実行空間に接続します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-130">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>](#bk_basic) <br/> |<span data-ttu-id="e83d7-131">Exchange Online サーバー</span><span class="sxs-lookup"><span data-stu-id="e83d7-131">Exchange Online servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell-LiveID`<br/><br/>`https://<server>/PowerShell-LiveID`  <br/> |
|[<span data-ttu-id="e83d7-132">証明書による認証を使用してリモートの実行空間に接続します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-132">Connect to a remote runspace by using certificate authentication</span></span>](#bk_cert) <br/> |<span data-ttu-id="e83d7-133">Exchange Online と Exchange オンプレミス サーバー</span><span class="sxs-lookup"><span data-stu-id="e83d7-133">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell`<br/><br/>`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |
|[<span data-ttu-id="e83d7-134">Kerberos 認証を使用して Exchange サーバーのリモートの実行空間に接続する</span><span class="sxs-lookup"><span data-stu-id="e83d7-134">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>](#bk_Kerberos) <br/> |<span data-ttu-id="e83d7-135">Exchange Online と Exchange オンプレミス サーバー</span><span class="sxs-lookup"><span data-stu-id="e83d7-135">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |

<span data-ttu-id="e83d7-136"><a name="bk_basic"> </a></span><span class="sxs-lookup"><span data-stu-id="e83d7-136"><a name="bk_basic"> </a></span></span>

### <a name="connect-to-a-remote-runspace-on-exchange-online-by-using-basic-authentication"></a><span data-ttu-id="e83d7-137">基本認証を使用して Exchange Online のリモートの実行空間に接続します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-137">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>

<span data-ttu-id="e83d7-138">次のコード例では、 **GetUsersUsingBasicAuth**メソッドを定義します。このメソッドは、基本認証を使用して、リモート exchange Online Server に Exchange 管理シェルの実行空間を作成します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-138">The following code example defines the **GetUsersUsingBasicAuth** method, which creates an Exchange Management Shell runspace on a remote Exchange Online server by using basic authentication.</span></span> <span data-ttu-id="e83d7-139">このメソッドは、「リモートの実行[空間からメールボックスユーザーのリストを取得](#bk_remote)する」で定義されているように、 **getuserinformation**メソッドを呼び出して、リモートサーバー上のユーザーの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-139">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="e83d7-140">このメソッドは、以下のパラメーターを必要とします。</span><span class="sxs-lookup"><span data-stu-id="e83d7-140">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="e83d7-141">**liveIDConnectionUri** &ndash;アプリケーションを認証する Exchange Online サーバーの URI を含む文字列。</span><span class="sxs-lookup"><span data-stu-id="e83d7-141">**liveIDConnectionUri** &ndash; A string that contains the URI of the Exchange Online server that will authenticate the application.</span></span> <span data-ttu-id="e83d7-142">Exchange Online が Office 365 で実行されている場合は、URI はになり `https://outlook.office365.com/PowerShell-LiveID` ます。それ以外の場合、uri は `https://<servername>/PowerShell-LiveID` です。</span><span class="sxs-lookup"><span data-stu-id="e83d7-142">If Exchange Online is running in Office 365, the URI is `https://outlook.office365.com/PowerShell-LiveID`; otherwise, the URI is `https://<servername>/PowerShell-LiveID`.</span></span> 
    
-  <span data-ttu-id="e83d7-143">**Schemauri** &ndash;Exchange 管理シェルスキーマを定義するスキーマドキュメントの URI を含む文字列。</span><span class="sxs-lookup"><span data-stu-id="e83d7-143">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="e83d7-144">スキーマ URI は `https://schemas.microsoft.com/powershell/Microsoft.Exchange` です。</span><span class="sxs-lookup"><span data-stu-id="e83d7-144">The schema URI is `https://schemas.microsoft.com/powershell/Microsoft.Exchange`.</span></span> 
    
-  <span data-ttu-id="e83d7-145">**資格情報** &ndash;アプリケーションを実行しているユーザーの資格情報を含む[PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="e83d7-145">**credentials** &ndash; A [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
-  <span data-ttu-id="e83d7-146">**count** &ndash;取得する Exchange メールボックスユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="e83d7-146">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
```cs
public Collection<PSObject> GetUsersUsingBasicAuth(
    string liveIDConnectionUri, string schemaUri, PSCredential credentials, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(liveIDConnectionUri),
        schemaUri, credentials);
    connectionInfo.AuthenticationMechanism = AuthenticationMechanism.Basic;
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```


```vb
  Function GetUsersUsingBasicAuth( _
    ByVal LiveIDConnectionUri As String, ByVal ScehmaUri As String, _
    ByVal Credentials As PSCredential, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo = _
        New WSManConnectionInfo(New Uri(LiveIDConnectionUri), ScehmaUri, Credentials)
    ConnectionInfo.AuthenticationMechanism = AuthenticationMechanism.Basic
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<span data-ttu-id="e83d7-147"><a name="bk_cert"> </a></span><span class="sxs-lookup"><span data-stu-id="e83d7-147"><a name="bk_cert"> </a></span></span>

### <a name="connect-to-a-remote-runspace-by-using-certificate-authentication"></a><span data-ttu-id="e83d7-148">証明書による認証を使用してリモートの実行空間に接続します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-148">Connect to a remote runspace by using certificate authentication</span></span>

<span data-ttu-id="e83d7-149">次のコード例では、 **GetUsersUsingCertificate**メソッドを定義します。このメソッドは、証明書を使用してリモートサーバー上に Exchange 管理シェルの実行空間を作成します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-149">The following code example defines the **GetUsersUsingCertificate** method, which creates an Exchange Management Shell runspace on a remote server by using a certificate.</span></span> <span data-ttu-id="e83d7-150">このメソッドは、「リモートの実行[空間からメールボックスユーザーのリストを取得](#bk_remote)する」で定義されているように、 **getuserinformation**メソッドを呼び出して、リモートサーバー上のユーザーの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-150">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="e83d7-151">このメソッドは、以下のパラメーターを必要とします。</span><span class="sxs-lookup"><span data-stu-id="e83d7-151">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="e83d7-152">**thumbprint** &ndash;アプリケーションを認証するために使用される証明書の拇印を含む文字列。</span><span class="sxs-lookup"><span data-stu-id="e83d7-152">**thumbprint** &ndash; A string that contains the thumbprint of the certificate that is used to authenticate the application.</span></span> 
    
-  <span data-ttu-id="e83d7-153">**Certconnectionuri** &ndash;証明書の認証を行うサーバーの URI を含む文字列。</span><span class="sxs-lookup"><span data-stu-id="e83d7-153">**certConnectionUri** &ndash; A string that contains the URI of the server that will authenticate the certificate.</span></span> <span data-ttu-id="e83d7-154">URI は、次の表に記載されているいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="e83d7-154">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="e83d7-155">**表1certConnectionUri Uri**</span><span class="sxs-lookup"><span data-stu-id="e83d7-155">**Table 1. certConnectionUri URIs**</span></span>

    |<span data-ttu-id="e83d7-156">**Server**</span><span class="sxs-lookup"><span data-stu-id="e83d7-156">**Server**</span></span>|<span data-ttu-id="e83d7-157">**URI**</span><span class="sxs-lookup"><span data-stu-id="e83d7-157">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="e83d7-158">SSL を使用しない Exchange サーバー</span><span class="sxs-lookup"><span data-stu-id="e83d7-158">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="e83d7-159">SSL を使用する Exchange サーバー</span><span class="sxs-lookup"><span data-stu-id="e83d7-159">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="e83d7-160">Office 365 の一部としての Exchange Online</span><span class="sxs-lookup"><span data-stu-id="e83d7-160">Exchange Online as part of Office 365</span></span>  <br/> |`https://outlook.office365.com/PowerShell`  <br/> |
   
- <span data-ttu-id="e83d7-161">**Schemauri** &ndash;Exchange 管理シェルスキーマを定義するスキーマドキュメントの URI を含む文字列。</span><span class="sxs-lookup"><span data-stu-id="e83d7-161">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="e83d7-162">スキーマ URI は https://schemas.microsoft.com/powershell/Microsoft.Exchange です。</span><span class="sxs-lookup"><span data-stu-id="e83d7-162">The schema URI is https://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="e83d7-163">**count** &ndash;取得する Exchange メールボックスユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="e83d7-163">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
```cs
public Collection<PSObject> GetUsersUsingCertificate(
    string thumbprint, string certConnectionUri, string schemaUri, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(certConnectionUri),
        schemaUri,
        thumbprint)
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```


```vb
  Function GetUsersUsingCertificate( _
    ByVal Thumbprint As String, ByVal CertConnectionUri As String, _
    ByVal SchemaUri As String, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo
    ConnectionInfo = New WSManConnectionInfo(New Uri(CertConnectionUri), SchemaUri, Thumbprint)
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<span data-ttu-id="e83d7-164"><a name="bk_Kerberos"> </a></span><span class="sxs-lookup"><span data-stu-id="e83d7-164"><a name="bk_Kerberos"> </a></span></span>

### <a name="connect-to-a-remote-runspace-on-an-exchange-server-by-using-kerberos-authentication"></a><span data-ttu-id="e83d7-165">Kerberos 認証を使用して Exchange サーバーのリモートの実行空間に接続する</span><span class="sxs-lookup"><span data-stu-id="e83d7-165">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>

<span data-ttu-id="e83d7-166">次のコード例では、 **GetUsersUsingKerberos**メソッドを定義します。このメソッドは、Kerberos 認証を使用してリモートサーバー上に Exchange 管理シェルの実行空間を作成します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-166">The following code example defines the **GetUsersUsingKerberos** method, which creates an Exchange Management Shell runspace on a remote server by using Kerberos authentication.</span></span> <span data-ttu-id="e83d7-167">このメソッドは、「リモートの実行[空間からメールボックスユーザーのリストを取得](#bk_remote)する」で定義されているように、 **getuserinformation**メソッドを呼び出して、リモートサーバー上のユーザーの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-167">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="e83d7-168">このメソッドは、以下のパラメーターを必要とします。</span><span class="sxs-lookup"><span data-stu-id="e83d7-168">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="e83d7-169">**kerberosUri** &ndash;アプリケーションを認証する Kerberos サーバーの URI を含む文字列。</span><span class="sxs-lookup"><span data-stu-id="e83d7-169">**kerberosUri** &ndash; A string that contains the URI of the Kerberos server that will authenticate the application.</span></span> <span data-ttu-id="e83d7-170">URI は、次の表に記載されているいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="e83d7-170">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="e83d7-171">**表2kerberosUri Uri**</span><span class="sxs-lookup"><span data-stu-id="e83d7-171">**Table 2. kerberosUri URIs**</span></span>

    |<span data-ttu-id="e83d7-172">**Server**</span><span class="sxs-lookup"><span data-stu-id="e83d7-172">**Server**</span></span>|<span data-ttu-id="e83d7-173">**URI**</span><span class="sxs-lookup"><span data-stu-id="e83d7-173">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="e83d7-174">SSL を使用しない Exchange サーバー</span><span class="sxs-lookup"><span data-stu-id="e83d7-174">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="e83d7-175">SSL を使用する Exchange サーバー</span><span class="sxs-lookup"><span data-stu-id="e83d7-175">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
   
- <span data-ttu-id="e83d7-176">**Schemauri** &ndash;Exchange 管理シェルスキーマを定義するスキーマドキュメントの URI を含む文字列。</span><span class="sxs-lookup"><span data-stu-id="e83d7-176">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="e83d7-177">スキーマ URI は https://schemas.microsoft.com/powershell/Microsoft.Exchange です。</span><span class="sxs-lookup"><span data-stu-id="e83d7-177">The schema URI is https://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="e83d7-178">**資格情報** &ndash;アプリケーションを実行しているユーザーの資格情報を含む[PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="e83d7-178">**credentials** &ndash; A [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
- <span data-ttu-id="e83d7-179">**count** &ndash;取得する Exchange メールボックスユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="e83d7-179">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
```cs
public Collection<PSObject> GetUsersUsingKerberos(
    string kerberosUri, string schemaUri, PSCredential credentials, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(kerberosUri),
        schemaUri, credentials);
    connectionInfo.AuthenticationMechanism = AuthenticationMechanism.Kerberos;
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```

```vb
  Function GetUsersUsingKerberos( _
    ByVal KerberosUri As String, ByVal ScehmaUri As String, _
    ByVal Credentials As PSCredential, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo = _
        New WSManConnectionInfo(New Uri(KerberosUri), ScehmaUri, Credentials)
    ConnectionInfo.AuthenticationMechanism = AuthenticationMechanism.Kerberos
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<span data-ttu-id="e83d7-180"><a name="bk_remote"> </a></span><span class="sxs-lookup"><span data-stu-id="e83d7-180"><a name="bk_remote"> </a></span></span>

## <a name="get-a-list-of-mailbox-users-from-a-remote-runspace"></a><span data-ttu-id="e83d7-181">リモートの実行空間からメールボックスのユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-181">Get a list of mailbox users from a remote runspace</span></span>

<span data-ttu-id="e83d7-182">次のコード例では、Exchange メールボックスユーザーを表す[PSObject](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx)インスタンスのコレクションを返す**getuserinformation**メソッドを定義します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-182">The following code example defines the **GetUserInformation** method, which returns a collection of [PSObject](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) instances that represent Exchange mailbox users.</span></span> <span data-ttu-id="e83d7-183">このメソッドは、 **GetUsersUsingBasicAuth**、 **GetUsersUsingCertificate**、および**GetUsersUsingKerberos**メソッドによって呼び出され、リモートサーバーからユーザーのリストを返します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-183">This method is called by the **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate**, and **GetUsersUsingKerberos** methods to return the list of users from the remote server.</span></span> 
  
<span data-ttu-id="e83d7-184">このメソッドは、以下のパラメーターを必要とします。</span><span class="sxs-lookup"><span data-stu-id="e83d7-184">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="e83d7-185">**count** &ndash;取得する Exchange メールボックスユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="e83d7-185">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
- <span data-ttu-id="e83d7-186">実行**空間** &ndash;リモート Exchange サーバーに対して確立されたリモートの実行空間。</span><span class="sxs-lookup"><span data-stu-id="e83d7-186">**runspace** &ndash; The remote runspace that is established for the remote Exchange server.</span></span> 
    
```cs
public Collection<PSObject> GetUserInformation(int count, Runspace runspace)
{
    using (PowerShell powershell = PowerShell.Create())
    {
        powershell.AddCommand("Get-Users");
        powershell.AddParameter("ResultSize", count);
        runspace.Open();
        powershell.Runspace = runspace;
        return powershell.Invoke();
    }
}
```

```vb
Function GetUserInformation(ByVal Count As Integer, ByVal RemoteRunspace As Runspace) As Collection(Of PSObject)
    Dim RemotePowerShell As PowerShell = PowerShell.Create
    RemotePowerShell.AddCommand("Get-Users")
    RemotePowerShell.AddParameter("ResultSize", Count)
    ' Open the remote runspace on the server.
    RemoteRunspace.Open()
    ' Associate the runspace with the Exchange Management Shell.
    RemotePowerShell.Runspace = RemoteRunspace
    ' Invoke the Exchange Management Shell to run the command.
    Return RemotePowerShell.Invoke
End Function

```

<span data-ttu-id="e83d7-187">**Getuserinformation**メソッドは、 _count ユーザー数_を超える数のメールボックスを返します。</span><span class="sxs-lookup"><span data-stu-id="e83d7-187">The **GetUserInformation** method will return no more than  _count_ mailbox users.</span></span> <span data-ttu-id="e83d7-188">この例のコードを簡略化するために、このメソッドは、返されるメールボックス ユーザーのフィルター処理やその他の方法による制限を行いません。</span><span class="sxs-lookup"><span data-stu-id="e83d7-188">To simplify the code for this example, the method does not filter or otherwise limit the mailbox users that are returned.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e83d7-189">関連項目</span><span class="sxs-lookup"><span data-stu-id="e83d7-189">See also</span></span>

- [<span data-ttu-id="e83d7-190">Exchange 管理シェル ツールの作成</span><span class="sxs-lookup"><span data-stu-id="e83d7-190">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="e83d7-191">Exchange 管理シェルコマンドレットの応答を使用する</span><span class="sxs-lookup"><span data-stu-id="e83d7-191">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)
    

