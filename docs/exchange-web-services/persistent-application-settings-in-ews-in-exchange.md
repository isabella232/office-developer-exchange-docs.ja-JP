---
title: Exchange の EWS の永続的なアプリケーションの設定
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 394d4e70-8517-4073-809a-5b61780ff923
description: Exchange で永続的なカスタム アプリケーション設定を作成するために EWS マネージ API または EWS アプリケーションが使用できる様々なオプションについて説明します。
ms.openlocfilehash: b384fd5608dc647950d7cd31e861e24c12e3316f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759179"
---
# <a name="persistent-application-settings-in-ews-in-exchange"></a>Exchange の EWS の永続的なアプリケーションの設定

Exchange で永続的なカスタム アプリケーション設定を作成するために EWS マネージ API または EWS アプリケーションが使用できる様々なオプションについて説明します。
  

  
メールボックス、またはメールボックスのフォルダーとアイテムのカスタム クライアント構成の同期を維持する最も簡単な方法は、Exchange サーバーにアプリケーション設定を保存することです。次のいずれかを使用して、メールボックスでこれらの設定を保持できます。  
  
- ユーザー構成オブジェクト
    
- 拡張プロパティ
    
- カスタム アイテム
    
## <a name="what-are-my-options-for-creating-persistent-application-settings"></a>永続的なアプリケーション設定を作成するためのオプション
<a name="Options"> </a>

ユーザー構成オブジェクトは、EWS クライアント アプリケーションの構成設定を格納するための最善のオプションです。また、拡張プロパティ、カスタム アイテム、または 3 つすべてを組み合わせて使用することもできます。設定のスコープ、および設定をその他のアプリケーションでも使用する必要があるかどうかに基づき、オプションを選びます。
  
**表 1. スコープに基づき永続的なアプリケーション設定を作成するための推奨オプション**

|**設定のスコープ**|**使う機能…**|**アクセス元**|
|:-----|:-----|:-----|
|アイテム  <br/> |既存の項目の拡張プロパティ。  <br/> |EWS アプリケーション。プロパティの識別子を知っている EWS クライアントのみが拡張プロパティにアクセスできます。  <br/> |
|Folder  <br/> |ターゲット フォルダーのユーザー構成オブジェクト。これは、フォルダーの表示設定を保存する場合に便利です。  <br/> |EWS アプリケーション。  <br/> |
|メールボックス  <br/> |既定の msgrootfolder フォルダーのユーザー構成オブジェクト。  <br/> |EWS アプリケーション。  <br/> |
   
### <a name="user-configuration-objects"></a>ユーザー構成オブジェクト
<a name="UserConfig"> </a>

ユーザー構成オブジェクトは、メールボックス内のフォルダーに関連付けられている特別なアイテムです。ユーザー構成オブジェクトは、フォルダー関連アイテムとも呼ばれ、通常、アプリケーションの設定を保持するのに最適なオプションです。構成情報がフォルダーまたはメールボックスに関連付けられている場合は、特にそう言えます。このオブジェクトは通常はエンド ユーザーに表示されません。データ ストリームやデータ ディクショナリをネイティブで格納することができるため、構成情報を格納するのに理想的です。ユーザー構成オブジェクトを使用する最善の方法は、構成のセットを XML ドキュメントに保存し、ユーザー構成のストリームのプロパティのいずれかにその情報を保存することです。
  
ユーザー構成オブジェクトは、メールボックスに格納されている他のアイテムの種類とは別にアクセスされます。 すべてのアイテムは [Folder.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=EXCHG.80%29.aspx) EWS マネージ API メソッド、または [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS 操作を利用して見つけることができますが、ユーザー構成オブジェクトを見つけるには **Associated** 検索走査オプションを使用する必要があります。 **Associated** 検索走査は、検索結果にユーザー構成オブジェクトしか含まれないことを示します。 EWS には、ユーザー構成オブジェクトに固有の操作のセットが含まれています。 
  
**表 1. ユーザー構成オブジェクトを操作するための EWS 操作と EWS マネージ API メソッド**

|**目的**|**使用する EWS 操作**|**使用する EWS マネージ API メソッド**|
|:-----|:-----|:-----|
|ユーザー構成オブジェクトを作成する  <br/> |[CreateUserConfiguration 操作](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) <br/> |[UserConfiguration.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) <br/> |
|ユーザー構成オブジェクトを取得する  <br/> |[GetUserConfiguration 操作](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |[UserConfiguration.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> [UserConfiguration.Load](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.userconfiguration.load%28v=exchg.80%29.aspx) <br/> |
|ユーザー構成オブジェクトを更新する  <br/> |[UpdateUserConfiguration 操作](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) <br/> |[UserConfiguration.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> |
|ユーザー構成オブジェクトを削除する  <br/> |[DeleteUserConfiguration 操作](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[UserConfiguration.Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |
   
> [!NOTE]
> EWS を使用して作成したユーザー構成オブジェクトは、"IPM.Configuration" で始まる [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) プレフィックスを持っています。 ユーザー構成オブジェクトの **ItemClass** は、ユーザー構成オブジェクトのプレフィックスとユーザー構成オブジェクトの名前です。 [Item.ItemClass](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) EWS マネージ API プロパティ、または **ItemClass** EWS 要素を使用して、定義済みのユーザー構成オブジェクトを検索できます。 
  
### <a name="extended-properties"></a>拡張プロパティ
<a name="ExtendedProperties"> </a>

アイテムの構成情報を保存する場合は、[拡張プロパティ](properties-and-extended-properties-in-ews-in-exchange.md)を使用します。 MAPI とは異なり、EWS は、アイテムのプロパティ バッグを返しません。 つまり、EWS のクライアントが拡張プロパティを見つけてアクセスするには、拡張プロパティの識別子を知っている必要があります。 ユーザー構成オブジェクト以外のアイテムに関する構成情報を保存する必要がある場合は、拡張プロパティを使用してカスタム プロパティを作成することが解決策になる可能性があります。 拡張プロパティを使用すると、アイテムの標準プロパティ セットの一部ではないプロパティの情報にアクセスしたり、それを保存したりできます。 
  
> [!IMPORTANT]
> Exchange データベースのスキーマでは、プロパティの数は有限です。 Exchange データベースのプロパティの識別子の最大数は、32,767 です。 拡張プロパティを使用して多数の設定を保存する場合は、単一の拡張プロパティを使用してこれらの設定を保存し、この最大値を超えないようにすることをお勧めします。 
  
[Item.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.update%28v=EXCHG.80%29.aspx) EWS マネージ API メソッドを使用するか、[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS 操作を使用して、ユーザー構成オブジェクトに拡張プロパティを設定できます。 
  
### <a name="custom-items"></a>カスタム アイテム
<a name="CustomItems"> </a>

カスタム アイテムは、情報の保存にも使用できます。既存のアイテムのプロパティは、構成情報を格納する用途にも使用できます。また、アプリケーション用の独自のプロパティを定義するために拡張プロパティを使用することができます。カスタム アイテムを使用して構成を保存することは、次の利点があります。  
  
- EWS をサポートする Exchange のすべてのバージョンで動作します。
    
- アイテムの拡張プロパティを使用しない場合、Exchange のプロパティのバジェットは変更されません。
    
## <a name="where-should-i-store-my-application-settings"></a>アプリケーション設定の保存場所
<a name="ApplicationSettingsLocation"> </a>

メールボックスのフォルダーとその中のアイテムは、メッセージのルート フォルダー内にあります。 このフォルダーは、EWS マネージ API の [WellKnownFolderName.msgfolderroot](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) の値によって識別されます。 MAPI の用語では、これはメールボックスの IPM サブツリーに相当します。 ユーザーがアクセスしているフォルダーに基づいてアプリケーションが表示設定を反映できるよう、ユーザー構成オブジェクトは UI ベースの設定を作成するためにしばしば使用されます。 フォルダー ベースの表示設定は通常、そのフォルダーに関連付けられているユーザー構成オブジェクトに設定されます。 しかし、設定をアプリケーション全体にグローバルに反映する場合もあります。 このケースでは、メッセージのルート フォルダーに設定を保存できます。 
  
ほとんどのユーザーは通常、ルート メールボックス フォルダーを意識せず、そこにアクセスすることはありません。 このフォルダーは、EWS マネージ API の [WellKnownFolderName.root](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) の値によって識別されます。 MAPI の用語では、これはメールボックスの IPM 以外のサブツリーに相当します。 エンド ユーザーが直接アクセスしない情報は、ルート メールボックス フォルダーに保存されます。 クライアント アプリケーションは通常このフォルダーにアクセスしないため、アプリケーションの設定をここに保存することをお勧めします。 
  
## <a name="version-differences"></a>バージョンの相違点
<a name="VersionDifferences"> </a>

ユーザー構成オブジェクトは、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2010 以降のバージョンの Exchange で利用できます。
  
## <a name="see-also"></a>関連項目


- [Exchange で EWS を使用して永続的なアプリケーションの設定を管理する](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
    
- [Exchange における EWS のプロパティと拡張プロパティ](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange で EWS を使用してフォルダーを操作する](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して Exchange メールボックス アイテムを操作する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    

