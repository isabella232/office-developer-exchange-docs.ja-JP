---
title: Exchange 管理シェルコマンドレットの応答を使用する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dac8e526-11c6-4c2e-b9a2-f016b1fc738a
description: Exchange の管理アプリケーションで、Exchange 管理シェル コマンドレットからの応答を使用する方法について説明します。
ms.openlocfilehash: c1b81356ab5dc288ab08287d47581871c36beb05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44435703"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a>Exchange 管理シェルコマンドレットの応答を使用する

Exchange の管理アプリケーションで、Exchange 管理シェル コマンドレットからの応答を使用する方法について説明します。
  
**適用対象:** Exchange Online |Exchange Server 2013 |Office 365
  
各 Exchange 管理シェルコマンドレットは、Exchange 管理シェル環境の任意のオブジェクトの一貫性のあるビューを提供する1つ以上の[PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx)インスタンスを返します。 この記事では、 **PSObject**インスタンスのプロパティを使用して、基になる Exchange SERVER 2013 API オブジェクトのプロパティ値を取得する方法について説明します。 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a>コマンドレットの応答を使用するための前提条件
<a name="prerequisites_bk"> </a>

コマンドレットの応答を使用するには、**System.Automation.Management** 名前空間の参照が必要です。 
  
> [!NOTE]
>  Visual Studio を使用してアプリケーションを作成するときには、System.Mangagement.Automation.dll アセンブリの参照をプロジェクトに追加する必要があります。アセンブリは次の場所のいずれかにあります。 
> - オペレーティング システムが Windows XP および Windows Vista の場合、Windows PowerShell のインストール ディレクトリ ($PSHOME)。 
> - オペレーティング システムが Windows 7 および Windows 8 の場合は次のフォルダー:Windows\assembly\GAC_MSIL\System.Management.Automation。 
  
## <a name="windows-powershell-remote-runspace"></a>Windows PowerShell のリモート実行空間
<a name="usingremoterunspace_bk"> </a>

Exchange 管理シェルでは、ローカル サーバーで実行されるコマンドであっても、すべてのコマンドに対して Windows PowerShell のリモート機能を使用します。その結果、Exchange 管理シェル コマンドレットからの応答は、すべてシリアル化された XML となります。つまり、その応答オブジェクトは、応答を生成するために使用した Exchange オブジェクトの種類は示しますが、Exchange オブジェクトの種類には型変換されません。代わりに、ユーザーご自身で、応答オブジェクトが公開するプロパティ バッグを使用して、Exchange オブジェクトの型から値を取得する必要があります。
  
応答オブジェクトのプロパティ バッグには、Exchange オブジェクト種類のパブリック プロパティまたはメソッドのごとにキー/値のペアが含まれています。応答オブジェクトには、基になる Exchange オブジェクト型の名前が含まれています。ユーザーはこの名前を使用して応答オブジェクトが表す Exchange オブジェクト型を決定し、プロパティを適切に抽出できます。ユーザーが適切に管理される型にプロパティ値を変換できるように、プロパティ バッグ内の各値には型情報も含まれています。
  
## <a name="use-the-cmdlet-response"></a>コマンドレット応答を使用する
<a name="usingPSObject_bk"> </a>

[PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx)クラスは、基になる EXCHANGE 2013 API オブジェクトの値を含む、次の3つのパブリックプロパティを公開します。[プロパティ](https://msdn.microsoft.com/library/system.management.automation.psobject.properties%28VS.85%29.aspx)、[メソッド](https://msdn.microsoft.com/library/system.management.automation.psobject.methods%28VS.85%29.aspx)、および[メンバー](https://msdn.microsoft.com/library/system.management.automation.psobject.members%28VS.85%29.aspx)。 Exchange 2013 API オブジェクトによって公開される各プロパティには、 **properties**および**Members**プロパティに対応するキーと値のペアがあります。 アプリケーションでは、プロパティの名前によって**Properties**コレクションのインデックスを作成し、プロパティの値を取得できます。 
  
**PSObject** インスタンスの **TypeNames** プロパティを使用して、**PSObject** インスタンスがカプセル化する、基になる Exchange オブジェクトの種類を決定できます。 **TypeNames** プロパティは文字列のコレクションであり、表される型のオブジェクト階層が含まれています。 これらの名前を使用して **PSObject** インスタンスが表すオブジェクトを決定し、適切にプロパティを抽出できるようにします。 
  
次のコード例では、コマンドレットの応答を使用して、コンソール上の **PSObject** インスタンスの **Properties** コレクションの内容を印刷します。 コード例には **System.Automation.Management** 名前空間の参照が必要です。 
  
```cs
foreach (PSPropertyInfo propertyInfo in psObject.Properties)
{
    Console.WriteLine(string.Format("{0}: {1}",
        propertyInfo.Name, propertyInfo.Value);
}
```

<br/>

```vb
For Each PropertyInfo As PSProperty In ObjectInfo.Properties
    Console.WriteLine(String.Format("{0}: {1}", PropertyInfo.Name, PropertyInfo.Value))
Next

```

## <a name="see-also"></a>関連項目

- [Exchange 管理シェル ツールの作成](create-exchange-management-shell-tools.md)   
- [Exchange 管理シェルを使用してメールユーザーの一覧を取得する](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

