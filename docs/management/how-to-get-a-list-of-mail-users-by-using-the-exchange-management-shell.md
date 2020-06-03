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
# <a name="get-a-list-of-mail-users-by-using-the-exchange-management-shell"></a>Exchange 管理シェルを使用してメールユーザーの一覧を取得する

Exchange 管理シェル コマンドレットを使用して、Exchange メールボックスのユーザーの一覧を取得するツールを作成する方法について説明します。
  
**適用対象:** Exchange Online |Exchange Server 2013 |Office 365 
  
Exchange 管理シェル コマンドレットを呼び出す管理ツールを使用して、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2013 以降のバージョンの Exchange からユーザーの一覧を取得することは、2 段階のプロセスです。 最初に、Exchange サーバー上のリモートの実行空間を確立し、次にリモートの実行空間内でユーザー情報を取得するコマンドレットを実行します。 

リモートの実行空間に接続するには、組織のセキュリティ要件を満たしている認証スキームを使用して、Exchange サーバーとの認証を行う必要があります。 

この記事では、リモートの実行空間を設定し、Exchange サーバーからユーザーの一覧を取得するための Exchange 管理シェル コマンドレットを実行するのに使用できるコード例を提供します。

<a name="bk_prerequisites"> </a>

## <a name="prerequisites-for-getting-a-list-of-mailbox-users"></a>メールボックスのユーザーの一覧を取得するための前提条件

このタスクを実行するには、次の名前空間への参照が必要です。
  
- **System.web モデル**
- **システム管理**
- **システムの管理**
- **システム管理の自動化**
    
> [!NOTE]
>  Visual Studio を使用してアプリケーションを作成する場合は、System.Management.Automation.dll アセンブリへの参照をプロジェクトに追加する必要があります。アセンブリは次の場所のいずれかにあります。
> - オペレーティング システムが Windows XP および Windows Vista の場合、Windows PowerShell のインストール ディレクトリ ($PSHOME)。
> - オペレーティング システムが Windows 7 および Windows 8 の場合は次のフォルダー:Windows\assembly\GAC_MSIL\System.Management.Automation。 
  
Exchange 管理シェルコマンドレットを自動化するアプリケーションを実行しているコンピューターの実行空間に、Exchange 2013 管理スナップインを読み込まないようにします。 代わりに、この記事で後述するように、アプリケーションはリモートの実行空間を作成する必要があります。

<a name="bk_gettinglistmailbox"> </a>

## <a name="connect-to-a-remote-runspace-on-an-exchange-server"></a>Exchange サーバーのリモートの実行空間に接続する

Exchange 管理シェル コマンドレットを使用するリモートの実行空間への接続に使用する方法は、使用している認証スキームによって異なります。このセクションでは、次の表に記載されている認証方法を使用している場合に、リモートの実行空間に接続する方法を示すコード例を提供します。
  
|**認証方法**|**適用対象**|**URI**|
|:-----|:-----|:-----|
|[基本認証を使用して Exchange Online のリモートの実行空間に接続します。](#bk_basic) <br/> |Exchange Online サーバー  <br/> |`https://outlook.office365.com/PowerShell-LiveID`<br/><br/>`https://<server>/PowerShell-LiveID`  <br/> |
|[証明書による認証を使用してリモートの実行空間に接続します。](#bk_cert) <br/> |Exchange Online と Exchange オンプレミス サーバー  <br/> |`https://outlook.office365.com/PowerShell`<br/><br/>`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |
|[Kerberos 認証を使用して Exchange サーバーのリモートの実行空間に接続する](#bk_Kerberos) <br/> |Exchange Online と Exchange オンプレミス サーバー  <br/> |`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |

<a name="bk_basic"> </a>

### <a name="connect-to-a-remote-runspace-on-exchange-online-by-using-basic-authentication"></a>基本認証を使用して Exchange Online のリモートの実行空間に接続します。

次のコード例では、 **GetUsersUsingBasicAuth**メソッドを定義します。このメソッドは、基本認証を使用して、リモート exchange Online Server に Exchange 管理シェルの実行空間を作成します。 このメソッドは、「リモートの実行[空間からメールボックスユーザーのリストを取得](#bk_remote)する」で定義されているように、 **getuserinformation**メソッドを呼び出して、リモートサーバー上のユーザーの一覧を返します。
  
このメソッドは、以下のパラメーターを必要とします。
  
-  **liveIDConnectionUri** &ndash;アプリケーションを認証する Exchange Online サーバーの URI を含む文字列。 Exchange Online が Office 365 で実行されている場合は、URI はになり `https://outlook.office365.com/PowerShell-LiveID` ます。それ以外の場合、uri は `https://<servername>/PowerShell-LiveID` です。 
    
-  **Schemauri** &ndash;Exchange 管理シェルスキーマを定義するスキーマドキュメントの URI を含む文字列。 スキーマ URI は `https://schemas.microsoft.com/powershell/Microsoft.Exchange` です。 
    
-  **資格情報** &ndash;アプリケーションを実行しているユーザーの資格情報を含む[PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx)オブジェクト。 
    
-  **count** &ndash;取得する Exchange メールボックスユーザーの数。 
    
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

次のコード例では、 **GetUsersUsingCertificate**メソッドを定義します。このメソッドは、証明書を使用してリモートサーバー上に Exchange 管理シェルの実行空間を作成します。 このメソッドは、「リモートの実行[空間からメールボックスユーザーのリストを取得](#bk_remote)する」で定義されているように、 **getuserinformation**メソッドを呼び出して、リモートサーバー上のユーザーの一覧を返します。
  
このメソッドは、以下のパラメーターを必要とします。
  
-  **thumbprint** &ndash;アプリケーションを認証するために使用される証明書の拇印を含む文字列。 
    
-  **Certconnectionuri** &ndash;証明書の認証を行うサーバーの URI を含む文字列。 URI は、次の表に記載されているいずれかになります。 
    
    **表1certConnectionUri Uri**

    |**Server**|**URI**|
    |:-----|:-----|
    |SSL を使用しない Exchange サーバー  <br/> |`http://<servername>/PowerShell`  <br/> |
    |SSL を使用する Exchange サーバー  <br/> |`https://<servername>/PowerShell`  <br/> |
    |Office 365 の一部としての Exchange Online  <br/> |`https://outlook.office365.com/PowerShell`  <br/> |
   
- **Schemauri** &ndash;Exchange 管理シェルスキーマを定義するスキーマドキュメントの URI を含む文字列。 スキーマ URI は https://schemas.microsoft.com/powershell/Microsoft.Exchange です。 
    
- **count** &ndash;取得する Exchange メールボックスユーザーの数。 
    
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

次のコード例では、 **GetUsersUsingKerberos**メソッドを定義します。このメソッドは、Kerberos 認証を使用してリモートサーバー上に Exchange 管理シェルの実行空間を作成します。 このメソッドは、「リモートの実行[空間からメールボックスユーザーのリストを取得](#bk_remote)する」で定義されているように、 **getuserinformation**メソッドを呼び出して、リモートサーバー上のユーザーの一覧を返します。
  
このメソッドは、以下のパラメーターを必要とします。
  
- **kerberosUri** &ndash;アプリケーションを認証する Kerberos サーバーの URI を含む文字列。 URI は、次の表に記載されているいずれかになります。 
    
    **表2kerberosUri Uri**

    |**Server**|**URI**|
    |:-----|:-----|
    |SSL を使用しない Exchange サーバー  <br/> |`http://<servername>/PowerShell`  <br/> |
    |SSL を使用する Exchange サーバー  <br/> |`https://<servername>/PowerShell`  <br/> |
   
- **Schemauri** &ndash;Exchange 管理シェルスキーマを定義するスキーマドキュメントの URI を含む文字列。 スキーマ URI は https://schemas.microsoft.com/powershell/Microsoft.Exchange です。 
    
- **資格情報** &ndash;アプリケーションを実行しているユーザーの資格情報を含む[PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx)オブジェクト。 
    
- **count** &ndash;取得する Exchange メールボックスユーザーの数。 
    
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

次のコード例では、Exchange メールボックスユーザーを表す[PSObject](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx)インスタンスのコレクションを返す**getuserinformation**メソッドを定義します。 このメソッドは、 **GetUsersUsingBasicAuth**、 **GetUsersUsingCertificate**、および**GetUsersUsingKerberos**メソッドによって呼び出され、リモートサーバーからユーザーのリストを返します。 
  
このメソッドは、以下のパラメーターを必要とします。
  
- **count** &ndash;取得する Exchange メールボックスユーザーの数。 
    
- 実行**空間** &ndash;リモート Exchange サーバーに対して確立されたリモートの実行空間。 
    
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

**Getuserinformation**メソッドは、 _count ユーザー数_を超える数のメールボックスを返します。 この例のコードを簡略化するために、このメソッドは、返されるメールボックス ユーザーのフィルター処理やその他の方法による制限を行いません。 
  
## <a name="see-also"></a>関連項目

- [Exchange 管理シェル ツールの作成](create-exchange-management-shell-tools.md)   
- [Exchange 管理シェルコマンドレットの応答を使用する](how-to-use-the-exchange-management-shell-cmdlet-response.md)
    

