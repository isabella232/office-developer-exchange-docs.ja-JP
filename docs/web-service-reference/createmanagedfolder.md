---
title: CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: cfdf01a9-0191-47c7-a7ad-5254d8bdee4a
description: CreateManagedFolder 要素は、管理されたカスタムフォルダーをメールボックスに追加する要求を定義します。
ms.openlocfilehash: 01fe8b7341c38ad33089c56271434ad3f9a4e5f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458363"
---
# <a name="createmanagedfolder"></a>CreateManagedFolder

**CreateManagedFolder**要素は、管理されたカスタムフォルダーをメールボックスに追加する要求を定義します。 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 **CreateManagedFolderRequestType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderNames](foldernames.md) <br/> |メールボックスに追加する名前付きの管理フォルダーの配列を格納します。  <br/> |
|[メールボックス](mailbox.md) <br/> |メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

要求を行っているユーザーのアカウントは、管理フォルダーが作成されたメールボックスに対して FullAccess アクセス許可を持っている必要があります。 Exchange 管理シェル**add-mailboxpermission**コマンドレットを使用して、フルアクセスのアクセス許可を割り当てることができます。 
  
Exchange Web サービスを使用して管理フォルダーをメールボックスに追加することはできますが、使用可能な管理フォルダーの一覧に Exchange Web サービスを使用してアクセスすることはできません。 利用可能な管理フォルダーの一覧を取得するには、Exchange 管理シェルコマンドレットの**取得**を使用します。 **Managedfolder コマンドレット**によって返されるリストには、管理されたカスタムフォルダーと管理された既定のフォルダーの両方が含まれます。 CreateManagedFolder 操作を使用して、 **managedcustomfolder**型のフォルダーのみをメールボックスに追加できます。 
  
> [!NOTE]
> また、Microsoft .NET Framework の System.directoryservices API を使用して、管理フォルダーの一覧を取得することもできます。 
  
[Findfolder 操作](findfolder-operation.md)を使用して、メールボックス内の管理されたフォルダーを検索できます。 管理フォルダーは、 [Baseshape](baseshape.md)要素を要求の allproperties に設定することで区別できます。 応答には、管理フォルダーを Exchange ストアフォルダーから区別する[Managedfolderinformation](managedfolderinformation.md)要素が含まれています。 他のフォルダーの種類を削除するのと同じ方法で、管理フォルダーを削除することができます。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateManagedFolder 操作](createmanagedfolder-operation.md)
  
[FindFolder 操作](findfolder-operation.md)


[フォルダーの検索](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[管理フォルダーの追加](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

