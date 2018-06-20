---
title: Exchange 管理シェルを使用してメール ユーザーの一覧を取得します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8b790dc8-5c4f-4acf-bbe7-63523395fbe7
description: Exchange 管理シェル コマンドレットを使用して、Exchange メールボックスのユーザーの一覧を取得するツールを作成する方法について説明します。
ms.openlocfilehash: 6f64330a11e372bffbea2fcd88bcfa0231ec0f28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759198"
---
# <a name="get-a-list-of-mail-users-by-using-the-exchange-management-shell"></a><span data-ttu-id="b77dd-103">Exchange 管理シェルを使用してメール ユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-103">Get a list of mail users by using the Exchange Management Shell</span></span>

<span data-ttu-id="b77dd-104">Exchange 管理シェル コマンドレットを使用して、Exchange メールボックスのユーザーの一覧を取得するツールを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-104">Learn how to use Exchange Management Shell cmdlets to create a tool that returns a list of Exchange mailbox users.</span></span>
  
<span data-ttu-id="b77dd-105">**に適用されます:** オンライン交換 |Exchange Server 2013年 |Office 365</span><span class="sxs-lookup"><span data-stu-id="b77dd-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span> 
  
<span data-ttu-id="b77dd-106">Exchange Online ユーザーの一覧を取得する、Office 365 の一部として Exchange のオンラインまたは、Exchange 管理シェル コマンドレットを呼び出すマネージ ツールを使用して Exchange 2013 で開始する Exchange のバージョンは、2 段階のプロセス。</span><span class="sxs-lookup"><span data-stu-id="b77dd-106">Getting a list of users from Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013 by using a managed tool that calls an Exchange Management Shell cmdlet is a two-step process.</span></span> <span data-ttu-id="b77dd-107">。 Exchange サーバー上のリモートの実行空間を確立する最初に、次に、リモートの実行空間内のユーザー情報を取得するコマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-107">First, you establish a remote runspace on an Exchange server; then, you run the cmdlet to retrieve the user information in the remote runspace.</span></span> 

<span data-ttu-id="b77dd-108">リモートの実行空間に接続するには、組織のセキュリティ要件を満たしている認証スキームを使用して Exchange サーバーとの認証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b77dd-108">To connect to the remote runspace, you have to authenticate with the Exchange server by using the authentication scheme that meets the security requirements of your organization.</span></span> 

<span data-ttu-id="b77dd-109">この資料では、リモートの実行空間を設定し、Exchange サーバーからユーザーの一覧を取得するのには、Exchange 管理シェル コマンドレットを実行するに使用できるコード例を提供します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-109">This article provides code examples that you can use to set up a remote runspace and run an Exchange Management Shell cmdlet to get a list of users from an Exchange server.</span></span>

<span data-ttu-id="b77dd-110"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="b77dd-110"></span></span>

## <a name="prerequisites-for-getting-a-list-of-mailbox-users"></a><span data-ttu-id="b77dd-111">メールボックスのユーザーの一覧を取得するための前提条件</span><span class="sxs-lookup"><span data-stu-id="b77dd-111">Prerequisites for getting a list of mailbox users</span></span>

<span data-ttu-id="b77dd-112">このタスクを実行するには、次の名前空間への参照が必要です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-112">To perform this task, you need a reference to the following namespaces:</span></span>
  
- <span data-ttu-id="b77dd-113">**System.Collections.ObjectModel**</span><span class="sxs-lookup"><span data-stu-id="b77dd-113">**System.Collections.ObjectModel**</span></span>
- <span data-ttu-id="b77dd-114">**System.Management.Automation**</span><span class="sxs-lookup"><span data-stu-id="b77dd-114">**System.Management.Automation**</span></span>
- <span data-ttu-id="b77dd-115">**System.Management.Automation.Remoting**</span><span class="sxs-lookup"><span data-stu-id="b77dd-115">**System.Management.Automation.Remoting**</span></span>
- <span data-ttu-id="b77dd-116">**System.Management.Automation.Runspaces**</span><span class="sxs-lookup"><span data-stu-id="b77dd-116">**System.Management.Automation.Runspaces**</span></span>
    
> [!NOTE]
>  <span data-ttu-id="b77dd-p102">Visual Studio を使用してアプリケーションを作成する場合は、System.Management.Automation.dll アセンブリへの参照をプロジェクトに追加する必要があります。アセンブリは次の場所のいずれかにあります。</span><span class="sxs-lookup"><span data-stu-id="b77dd-p102">When you are using Visual Studio to create an application, you must add a reference to the System.Management.Automation.dll assembly to the project. The assembly can be found in one of the following locations:</span></span>
> - <span data-ttu-id="b77dd-119">オペレーティング システムが Windows XP および Windows Vista の場合、Windows PowerShell のインストール ディレクトリ ($PSHOME)。</span><span class="sxs-lookup"><span data-stu-id="b77dd-119">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span>
> - <span data-ttu-id="b77dd-120">オペレーティング システムが Windows 7 および Windows 8 の場合は次のフォルダー:Windows\assembly\GAC_MSIL\System.Management.Automation。</span><span class="sxs-lookup"><span data-stu-id="b77dd-120">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
<span data-ttu-id="b77dd-121">読み込まない Exchange 2013 の管理] スナップインで、Exchange 管理シェル コマンドレットを自動化するアプリケーションを実行するコンピューターで実行空間にします。</span><span class="sxs-lookup"><span data-stu-id="b77dd-121">Do not load the Exchange 2013 Management snap-in into the runspace on computers that are running applications that automate Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="b77dd-122">代わりに、アプリケーションはこの資料で後述するよう、リモートの実行空間を作成しています。</span><span class="sxs-lookup"><span data-stu-id="b77dd-122">The application should instead create a remote runspace, as described later in this article.</span></span>

<span data-ttu-id="b77dd-123"><a name="bk_gettinglistmailbox"> </a></span><span class="sxs-lookup"><span data-stu-id="b77dd-123"></span></span>

## <a name="connect-to-a-remote-runspace-on-an-exchange-server"></a><span data-ttu-id="b77dd-124">Exchange サーバーのリモートの実行空間に接続する</span><span class="sxs-lookup"><span data-stu-id="b77dd-124">Connect to a remote runspace on an Exchange server</span></span>

<span data-ttu-id="b77dd-p104">Exchange 管理シェル コマンドレットを使用するリモートの実行空間への接続に使用する方法は、使用している認証スキームによって異なります。このセクションでは、次の表に記載されている認証方法を使用している場合に、リモートの実行空間に接続する方法を示すコード例を提供します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-p104">The method that you use to connect to a remote runspace to use an Exchange Management Shell cmdlet varies based on the authentication scheme that you are using. This section provides code examples that show how to connect to a remote runspace when you are using an authentication method listed in the following table.</span></span>
  
|<span data-ttu-id="b77dd-127">**認証方法**</span><span class="sxs-lookup"><span data-stu-id="b77dd-127">**Authentication method**</span></span>|<span data-ttu-id="b77dd-128">**適用されます。**</span><span class="sxs-lookup"><span data-stu-id="b77dd-128">**Applies to**</span></span>|<span data-ttu-id="b77dd-129">**URI**</span><span class="sxs-lookup"><span data-stu-id="b77dd-129">**URI**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="b77dd-130">基本認証を使用して Exchange Online にリモートの実行空間に接続します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-130">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>](#bk_basic) <br/> |<span data-ttu-id="b77dd-131">Exchange Online サーバー</span><span class="sxs-lookup"><span data-stu-id="b77dd-131">Exchange Online servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell-LiveID`<br/><br/>`https://<server>/PowerShell-LiveID`  <br/> |
|[<span data-ttu-id="b77dd-132">証明書による認証を使用してリモートの実行空間に接続します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-132">Connect to a remote runspace by using certificate authentication</span></span>](#bk_cert) <br/> |<span data-ttu-id="b77dd-133">Exchange Online と Exchange オンプレミス サーバー</span><span class="sxs-lookup"><span data-stu-id="b77dd-133">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell`<br/><br/>`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |
|[<span data-ttu-id="b77dd-134">Kerberos 認証を使用して Exchange サーバー上のリモートの実行空間に接続します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-134">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>](#bk_Kerberos) <br/> |<span data-ttu-id="b77dd-135">Exchange Online と Exchange オンプレミス サーバー</span><span class="sxs-lookup"><span data-stu-id="b77dd-135">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |

<span data-ttu-id="b77dd-136"><a name="bk_basic"> </a></span><span class="sxs-lookup"><span data-stu-id="b77dd-136"></span></span>

### <a name="connect-to-a-remote-runspace-on-exchange-online-by-using-basic-authentication"></a><span data-ttu-id="b77dd-137">基本認証を使用して Exchange Online のリモートの実行空間に接続します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-137">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>

<span data-ttu-id="b77dd-138">次のコード例では、 **GetUsersUsingBasicAuth**メソッドは、基本認証を使用して、リモートのオンラインの Exchange サーバー上で Exchange 管理シェルの実行空間を作成するを定義します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-138">The following code example defines the **GetUsersUsingBasicAuth** method, which creates an Exchange Management Shell runspace on a remote Exchange Online server by using basic authentication.</span></span> <span data-ttu-id="b77dd-139">メソッド メソッドを呼び出して、 **GetUserInformation** 、リモート サーバー上のユーザーの一覧を取得するのには、[リモートの実行空間からのユーザーのメールボックスの一覧を取得する](#bk_remote)には、セクションで定義されています。</span><span class="sxs-lookup"><span data-stu-id="b77dd-139">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="b77dd-140">このメソッドは、以下のパラメーターを必要とします。</span><span class="sxs-lookup"><span data-stu-id="b77dd-140">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="b77dd-141">**liveIDConnectionUri**&ndash;アプリケーションを認証するオンラインの Exchange サーバーの URI を含む文字列です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-141">**liveIDConnectionUri** &ndash; A string that contains the URI of the Exchange Online server that will authenticate the application.</span></span> <span data-ttu-id="b77dd-142">Office 365 のオンラインの Exchange を実行する場合、URI は、 https://outlook.office365.com/PowerShell-LiveID。それ以外の場合、URI は、https://\<サーバー名\>/PowerShell-LiveID。</span><span class="sxs-lookup"><span data-stu-id="b77dd-142">If Exchange Online is running in Office 365, the URI is https://outlook.office365.com/PowerShell-LiveID; otherwise, the URI is https://\<servername\>/PowerShell-LiveID.</span></span> 
    
-  <span data-ttu-id="b77dd-143">**schemaUri**&ndash; Exchange 管理シェルのスキーマを定義するスキーマ ドキュメントの URI を含む文字列です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-143">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="b77dd-144">スキーマの URI は、 http://schemas.microsoft.com/powershell/Microsoft.Exchange。</span><span class="sxs-lookup"><span data-stu-id="b77dd-144">The schema URI is http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
-  <span data-ttu-id="b77dd-145">**資格情報**&ndash;アプリケーションを実行したユーザーの資格情報を格納する[PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b77dd-145">**credentials** &ndash; A [PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
-  <span data-ttu-id="b77dd-146">**カウント**&ndash;取得するのには Exchange メールボックス ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-146">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
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

<span data-ttu-id="b77dd-147"><a name="bk_cert"> </a></span><span class="sxs-lookup"><span data-stu-id="b77dd-147"></span></span>

### <a name="connect-to-a-remote-runspace-by-using-certificate-authentication"></a><span data-ttu-id="b77dd-148">証明書による認証を使用してリモートの実行空間に接続します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-148">Connect to a remote runspace by using certificate authentication</span></span>

<span data-ttu-id="b77dd-149">次のコード例は、証明書を使用して、リモート サーバー上の Exchange 管理シェルの実行空間を作成する、 **GetUsersUsingCertificate**メソッドを定義します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-149">The following code example defines the **GetUsersUsingCertificate** method, which creates an Exchange Management Shell runspace on a remote server by using a certificate.</span></span> <span data-ttu-id="b77dd-150">メソッド メソッドを呼び出して、 **GetUserInformation** 、リモート サーバー上のユーザーの一覧を取得するのには、[リモートの実行空間からのユーザーのメールボックスの一覧を取得する](#bk_remote)には、セクションで定義されています。</span><span class="sxs-lookup"><span data-stu-id="b77dd-150">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="b77dd-151">このメソッドは、以下のパラメーターを必要とします。</span><span class="sxs-lookup"><span data-stu-id="b77dd-151">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="b77dd-152">**拇印**&ndash;アプリケーションを認証するために使用される証明書の拇印を含む文字列です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-152">**thumbprint** &ndash; A string that contains the thumbprint of the certificate that is used to authenticate the application.</span></span> 
    
-  <span data-ttu-id="b77dd-153">**certConnectionUri**&ndash;証明書を認証するサーバーの URI を含む文字列です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-153">**certConnectionUri** &ndash; A string that contains the URI of the server that will authenticate the certificate.</span></span> <span data-ttu-id="b77dd-154">URI は、次の表に記載されているのいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="b77dd-154">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="b77dd-155">**表 1 です。certConnectionUri Uri**</span><span class="sxs-lookup"><span data-stu-id="b77dd-155">**Table 1. certConnectionUri URIs**</span></span>

    |<span data-ttu-id="b77dd-156">**Server**</span><span class="sxs-lookup"><span data-stu-id="b77dd-156">**Server**</span></span>|<span data-ttu-id="b77dd-157">**URI**</span><span class="sxs-lookup"><span data-stu-id="b77dd-157">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="b77dd-158">SSL を使用しない Exchange サーバー</span><span class="sxs-lookup"><span data-stu-id="b77dd-158">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="b77dd-159">SSL を使用する Exchange サーバー</span><span class="sxs-lookup"><span data-stu-id="b77dd-159">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="b77dd-160">Office 365 の一部としての Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b77dd-160">Exchange Online as part of Office 365</span></span>  <br/> |`https://outlook.office365.com/PowerShell`  <br/> |
   
- <span data-ttu-id="b77dd-161">**schemaUri**&ndash; Exchange 管理シェルのスキーマを定義するスキーマ ドキュメントの URI を含む文字列です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-161">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="b77dd-162">スキーマの URI は、 http://schemas.microsoft.com/powershell/Microsoft.Exchange。</span><span class="sxs-lookup"><span data-stu-id="b77dd-162">The schema URI is http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="b77dd-163">**カウント**&ndash;取得するのには Exchange メールボックス ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-163">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
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

<span data-ttu-id="b77dd-164"><a name="bk_Kerberos"> </a></span><span class="sxs-lookup"><span data-stu-id="b77dd-164"></span></span>

### <a name="connect-to-a-remote-runspace-on-an-exchange-server-by-using-kerberos-authentication"></a><span data-ttu-id="b77dd-165">Kerberos 認証を使用して Exchange サーバーのリモートの実行空間に接続する</span><span class="sxs-lookup"><span data-stu-id="b77dd-165">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>

<span data-ttu-id="b77dd-166">次のコード例は、Kerberos 認証を使用してリモート サーバー上で Exchange 管理シェルの実行空間を作成する、 **GetUsersUsingKerberos**メソッドを定義します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-166">The following code example defines the **GetUsersUsingKerberos** method, which creates an Exchange Management Shell runspace on a remote server by using Kerberos authentication.</span></span> <span data-ttu-id="b77dd-167">メソッド メソッドを呼び出して、 **GetUserInformation** 、リモート サーバー上のユーザーの一覧を取得するのには、[リモートの実行空間からのユーザーのメールボックスの一覧を取得する](#bk_remote)には、セクションで定義されています。</span><span class="sxs-lookup"><span data-stu-id="b77dd-167">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="b77dd-168">このメソッドは、以下のパラメーターを必要とします。</span><span class="sxs-lookup"><span data-stu-id="b77dd-168">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="b77dd-169">**kerberosUri**&ndash;アプリケーションは、認証を Kerberos サーバーの URI を含む文字列です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-169">**kerberosUri** &ndash; A string that contains the URI of the Kerberos server that will authenticate the application.</span></span> <span data-ttu-id="b77dd-170">URI は、次の表に記載されているのいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="b77dd-170">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="b77dd-171">**表 2 になります。kerberosUri Uri**</span><span class="sxs-lookup"><span data-stu-id="b77dd-171">**Table 2. kerberosUri URIs**</span></span>

    |<span data-ttu-id="b77dd-172">**Server**</span><span class="sxs-lookup"><span data-stu-id="b77dd-172">**Server**</span></span>|<span data-ttu-id="b77dd-173">**URI**</span><span class="sxs-lookup"><span data-stu-id="b77dd-173">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="b77dd-174">SSL を使用しない Exchange サーバー</span><span class="sxs-lookup"><span data-stu-id="b77dd-174">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="b77dd-175">SSL を使用する Exchange サーバー</span><span class="sxs-lookup"><span data-stu-id="b77dd-175">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
   
- <span data-ttu-id="b77dd-176">**schemaUri**&ndash; Exchange 管理シェルのスキーマを定義するスキーマ ドキュメントの URI を含む文字列です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-176">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="b77dd-177">スキーマの URI は、 http://schemas.microsoft.com/powershell/Microsoft.Exchange。</span><span class="sxs-lookup"><span data-stu-id="b77dd-177">The schema URI is http://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="b77dd-178">**資格情報**&ndash;アプリケーションを実行したユーザーの資格情報を格納する[PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b77dd-178">**credentials** &ndash; A [PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
- <span data-ttu-id="b77dd-179">**カウント**&ndash;取得するのには Exchange メールボックス ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-179">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
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

<span data-ttu-id="b77dd-180"><a name="bk_remote"> </a></span><span class="sxs-lookup"><span data-stu-id="b77dd-180"></span></span>

## <a name="get-a-list-of-mailbox-users-from-a-remote-runspace"></a><span data-ttu-id="b77dd-181">リモートの実行空間からメールボックスのユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-181">Get a list of mailbox users from a remote runspace</span></span>

<span data-ttu-id="b77dd-182">コード例を次は、Exchange メールボックス ユーザーを表す[PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx)インスタンスのコレクションを取得する、 **GetUserInformation**メソッドを定義します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-182">The following code example defines the **GetUserInformation** method, which returns a collection of [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) instances that represent Exchange mailbox users.</span></span> <span data-ttu-id="b77dd-183">このメソッドは、リモート サーバーからユーザーの一覧を取得する**GetUsersUsingBasicAuth**、 **GetUsersUsingCertificate**、および**GetUsersUsingKerberos**のメソッドによって呼び出されます。</span><span class="sxs-lookup"><span data-stu-id="b77dd-183">This method is called by the **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate**, and **GetUsersUsingKerberos** methods to return the list of users from the remote server.</span></span> 
  
<span data-ttu-id="b77dd-184">このメソッドは、以下のパラメーターを必要とします。</span><span class="sxs-lookup"><span data-stu-id="b77dd-184">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="b77dd-185">**カウント**&ndash;取得するのには Exchange メールボックス ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-185">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
- <span data-ttu-id="b77dd-186">**実行空間**&ndash;リモートの Exchange サーバーに対して確立されているリモートの実行空間です。</span><span class="sxs-lookup"><span data-stu-id="b77dd-186">**runspace** &ndash; The remote runspace that is established for the remote Exchange server.</span></span> 
    
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

<span data-ttu-id="b77dd-187">**GetUserInformation**メソッドはユーザーのメールボックスに以上の_数_に戻ります。</span><span class="sxs-lookup"><span data-stu-id="b77dd-187">The **GetUserInformation** method will return no more than  _count_ mailbox users.</span></span> <span data-ttu-id="b77dd-188">この例のコードを簡略化するには、メソッドをフィルター処理したりしないそれ以外の場合に返されるメールボックス ユーザーを制限します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-188">To simplify the code for this example, the method does not filter or otherwise limit the mailbox users that are returned.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b77dd-189">関連項目</span><span class="sxs-lookup"><span data-stu-id="b77dd-189">See also</span></span>

- [<span data-ttu-id="b77dd-190">Exchange 管理シェルのツールを作成します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-190">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="b77dd-191">Exchange 管理シェル コマンドレットの応答を使用します。</span><span class="sxs-lookup"><span data-stu-id="b77dd-191">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)
    

