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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759198"
---
# <a name="get-a-list-of-mail-users-by-using-the-exchange-management-shell"></a>Exchange 管理シェルを使用してメール ユーザーの一覧を取得します。

Exchange 管理シェル コマンドレットを使用して、Exchange メールボックスのユーザーの一覧を取得するツールを作成する方法について説明します。
  
**に適用されます:** オンライン交換 |Exchange Server 2013年 |Office 365 
  
Exchange Online ユーザーの一覧を取得する、Office 365 の一部として Exchange のオンラインまたは、Exchange 管理シェル コマンドレットを呼び出すマネージ ツールを使用して Exchange 2013 で開始する Exchange のバージョンは、2 段階のプロセス。 。 Exchange サーバー上のリモートの実行空間を確立する最初に、次に、リモートの実行空間内のユーザー情報を取得するコマンドレットを実行します。 

リモートの実行空間に接続するには、組織のセキュリティ要件を満たしている認証スキームを使用して Exchange サーバーとの認証する必要があります。 

この資料では、リモートの実行空間を設定し、Exchange サーバーからユーザーの一覧を取得するのには、Exchange 管理シェル コマンドレットを実行するに使用できるコード例を提供します。

<a name="bk_prerequisites"> </a>

## <a name="prerequisites-for-getting-a-list-of-mailbox-users"></a>メールボックスのユーザーの一覧を取得するための前提条件

このタスクを実行するには、次の名前空間への参照が必要です。
  
- **System.Collections.ObjectModel**
- **System.Management.Automation**
- **System.Management.Automation.Remoting**
- **System.Management.Automation.Runspaces**
    
> [!NOTE]
>  Visual Studio を使用してアプリケーションを作成する場合は、System.Management.Automation.dll アセンブリへの参照をプロジェクトに追加する必要があります。アセンブリは次の場所のいずれかにあります。
> - オペレーティング システムが Windows XP および Windows Vista の場合、Windows PowerShell のインストール ディレクトリ ($PSHOME)。
> - オペレーティング システムが Windows 7 および Windows 8 の場合は次のフォルダー:Windows\assembly\GAC_MSIL\System.Management.Automation。 
  
読み込まない Exchange 2013 の管理] スナップインで、Exchange 管理シェル コマンドレットを自動化するアプリケーションを実行するコンピューターで実行空間にします。 代わりに、アプリケーションはこの資料で後述するよう、リモートの実行空間を作成しています。

<a name="bk_gettinglistmailbox"> </a>

## <a name="connect-to-a-remote-runspace-on-an-exchange-server"></a>Exchange サーバーのリモートの実行空間に接続する

Exchange 管理シェル コマンドレットを使用するリモートの実行空間への接続に使用する方法は、使用している認証スキームによって異なります。このセクションでは、次の表に記載されている認証方法を使用している場合に、リモートの実行空間に接続する方法を示すコード例を提供します。
  
|**認証方法**|**適用されます。**|**URI**|
|:-----|:-----|:-----|
|[基本認証を使用して Exchange Online にリモートの実行空間に接続します。](#bk_basic) <br/> |Exchange Online サーバー  <br/> |`https://outlook.office365.com/PowerShell-LiveID`<br/><br/>`https://<server>/PowerShell-LiveID`  <br/> |
|[証明書による認証を使用してリモートの実行空間に接続します。](#bk_cert) <br/> |Exchange Online と Exchange オンプレミス サーバー  <br/> |`https://outlook.office365.com/PowerShell`<br/><br/>`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |
|[Kerberos 認証を使用して Exchange サーバー上のリモートの実行空間に接続します。](#bk_Kerberos) <br/> |Exchange Online と Exchange オンプレミス サーバー  <br/> |`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |

<a name="bk_basic"> </a>

### <a name="connect-to-a-remote-runspace-on-exchange-online-by-using-basic-authentication"></a>基本認証を使用して Exchange Online のリモートの実行空間に接続します。

次のコード例では、 **GetUsersUsingBasicAuth**メソッドは、基本認証を使用して、リモートのオンラインの Exchange サーバー上で Exchange 管理シェルの実行空間を作成するを定義します。 メソッド メソッドを呼び出して、 **GetUserInformation** 、リモート サーバー上のユーザーの一覧を取得するのには、[リモートの実行空間からのユーザーのメールボックスの一覧を取得する](#bk_remote)には、セクションで定義されています。
  
このメソッドは、以下のパラメーターを必要とします。
  
-  **liveIDConnectionUri**&ndash;アプリケーションを認証するオンラインの Exchange サーバーの URI を含む文字列です。 Office 365 のオンラインの Exchange を実行する場合、URI は、 https://outlook.office365.com/PowerShell-LiveID。それ以外の場合、URI は、https://\<サーバー名\>/PowerShell-LiveID。 
    
-  **schemaUri**&ndash; Exchange 管理シェルのスキーマを定義するスキーマ ドキュメントの URI を含む文字列です。 スキーマの URI は、 http://schemas.microsoft.com/powershell/Microsoft.Exchange。 
    
-  **資格情報**&ndash;アプリケーションを実行したユーザーの資格情報を格納する[PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx)オブジェクトです。 
    
-  **カウント**&ndash;取得するのには Exchange メールボックス ユーザーの数です。 
    
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

<a name="bk_cert"> </a>

### <a name="connect-to-a-remote-runspace-by-using-certificate-authentication"></a>証明書による認証を使用してリモートの実行空間に接続します。

次のコード例は、証明書を使用して、リモート サーバー上の Exchange 管理シェルの実行空間を作成する、 **GetUsersUsingCertificate**メソッドを定義します。 メソッド メソッドを呼び出して、 **GetUserInformation** 、リモート サーバー上のユーザーの一覧を取得するのには、[リモートの実行空間からのユーザーのメールボックスの一覧を取得する](#bk_remote)には、セクションで定義されています。
  
このメソッドは、以下のパラメーターを必要とします。
  
-  **拇印**&ndash;アプリケーションを認証するために使用される証明書の拇印を含む文字列です。 
    
-  **certConnectionUri**&ndash;証明書を認証するサーバーの URI を含む文字列です。 URI は、次の表に記載されているのいずれかになります。 
    
    **表 1 です。certConnectionUri Uri**

    |**Server**|**URI**|
    |:-----|:-----|
    |SSL を使用しない Exchange サーバー  <br/> |`http://<servername>/PowerShell`  <br/> |
    |SSL を使用する Exchange サーバー  <br/> |`https://<servername>/PowerShell`  <br/> |
    |Office 365 の一部としての Exchange Online  <br/> |`https://outlook.office365.com/PowerShell`  <br/> |
   
- **schemaUri**&ndash; Exchange 管理シェルのスキーマを定義するスキーマ ドキュメントの URI を含む文字列です。 スキーマの URI は、 http://schemas.microsoft.com/powershell/Microsoft.Exchange。 
    
- **カウント**&ndash;取得するのには Exchange メールボックス ユーザーの数です。 
    
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

<a name="bk_Kerberos"> </a>

### <a name="connect-to-a-remote-runspace-on-an-exchange-server-by-using-kerberos-authentication"></a>Kerberos 認証を使用して Exchange サーバーのリモートの実行空間に接続する

次のコード例は、Kerberos 認証を使用してリモート サーバー上で Exchange 管理シェルの実行空間を作成する、 **GetUsersUsingKerberos**メソッドを定義します。 メソッド メソッドを呼び出して、 **GetUserInformation** 、リモート サーバー上のユーザーの一覧を取得するのには、[リモートの実行空間からのユーザーのメールボックスの一覧を取得する](#bk_remote)には、セクションで定義されています。
  
このメソッドは、以下のパラメーターを必要とします。
  
- **kerberosUri**&ndash;アプリケーションは、認証を Kerberos サーバーの URI を含む文字列です。 URI は、次の表に記載されているのいずれかになります。 
    
    **表 2 になります。kerberosUri Uri**

    |**Server**|**URI**|
    |:-----|:-----|
    |SSL を使用しない Exchange サーバー  <br/> |`http://<servername>/PowerShell`  <br/> |
    |SSL を使用する Exchange サーバー  <br/> |`https://<servername>/PowerShell`  <br/> |
   
- **schemaUri**&ndash; Exchange 管理シェルのスキーマを定義するスキーマ ドキュメントの URI を含む文字列です。 スキーマの URI は、 http://schemas.microsoft.com/powershell/Microsoft.Exchange。 
    
- **資格情報**&ndash;アプリケーションを実行したユーザーの資格情報を格納する[PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx)オブジェクトです。 
    
- **カウント**&ndash;取得するのには Exchange メールボックス ユーザーの数です。 
    
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

<a name="bk_remote"> </a>

## <a name="get-a-list-of-mailbox-users-from-a-remote-runspace"></a>リモートの実行空間からメールボックスのユーザーの一覧を取得します。

コード例を次は、Exchange メールボックス ユーザーを表す[PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx)インスタンスのコレクションを取得する、 **GetUserInformation**メソッドを定義します。 このメソッドは、リモート サーバーからユーザーの一覧を取得する**GetUsersUsingBasicAuth**、 **GetUsersUsingCertificate**、および**GetUsersUsingKerberos**のメソッドによって呼び出されます。 
  
このメソッドは、以下のパラメーターを必要とします。
  
- **カウント**&ndash;取得するのには Exchange メールボックス ユーザーの数です。 
    
- **実行空間**&ndash;リモートの Exchange サーバーに対して確立されているリモートの実行空間です。 
    
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

**GetUserInformation**メソッドはユーザーのメールボックスに以上の_数_に戻ります。 この例のコードを簡略化するには、メソッドをフィルター処理したりしないそれ以外の場合に返されるメールボックス ユーザーを制限します。 
  
## <a name="see-also"></a>関連項目

- [Exchange 管理シェルのツールを作成します。](create-exchange-management-shell-tools.md)   
- [Exchange 管理シェル コマンドレットの応答を使用します。](how-to-use-the-exchange-management-shell-cmdlet-response.md)
    

