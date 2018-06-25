---
title: Exchange 管理シェル コマンドレットの応答を使用します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dac8e526-11c6-4c2e-b9a2-f016b1fc738a
description: Exchange の管理アプリケーションで、Exchange 管理シェル コマンドレットからの応答を使用する方法について説明します。
ms.openlocfilehash: 5edf75afd556f67e815bc519c87586f2f62f057b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759194"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a>Exchange 管理シェル コマンドレットの応答を使用します。

Exchange の管理アプリケーションで、Exchange 管理シェル コマンドレットからの応答を使用する方法について説明します。
  
**に適用されます:** オンライン交換 |Exchange Server 2013年 |Office 365
  
各 Exchange 管理シェル コマンドレットは、Exchange 管理シェル環境での任意のオブジェクトの整合性のとれたビューを提供する 1 つまたは複数の[PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx)インスタンスを返します。 **PSObject**インスタンスのプロパティを使用して、基になる Exchange Server 2013 API オブジェクトのプロパティ値を取得する方法について説明します。 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a>コマンドレットの応答を使用するための前提条件
<a name="prerequisites_bk"> </a>

コマンドレットの応答を使用するには、 **System.Automation.Management**名前空間への参照が必要です。 
  
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

[PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx)クラスを基になる Exchange 2013 の API のオブジェクトの値を含む、次の 3 つパブリック プロパティを公開する:[プロパティ](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.properties%28VS.85%29.aspx)、[メソッド](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.methods%28VS.85%29.aspx)、および[メンバー](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.members%28VS.85%29.aspx)。 Exchange 2013 API オブジェクトによって公開されている各プロパティには、**プロパティ**と**メンバー**のプロパティで対応するキー/値のペアがあります。 アプリケーションは、プロパティの値を取得するプロパティの名前を**Properties**コレクションのインデックスを作成できます。 
  
**PSObject**インスタンスの**型名**プロパティを使用するには**PSObject**のインスタンスによってカプセル化された基になる Exchange オブジェクトの種類を決定します。 **型名**のプロパティは、表される型のオブジェクトの階層を含む文字列のコレクションです。 これらの名前を使用するには、適切なプロパティを抽出することができますように**PSObject**のインスタンスによって表されるオブジェクトを決定します。 
  
次のコード例は、 **PSObject**インスタンスの**プロパティ**のコレクションの内容をコンソールに印刷するのには、コマンドレットの応答を使用します。 コード例では、 **System.Automation.Management**名前空間への参照が必要です。 
  
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

- [Exchange 管理シェルのツールを作成します。](create-exchange-management-shell-tools.md)   
- [Exchange 管理シェルを使用してメール ユーザーの一覧を取得します。](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

