---
title: CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: cfdf01a9-0191-47c7-a7ad-5254d8bdee4a
description: CreateManagedFolder 要素は、管理されたカスタム フォルダーをメールボックスに追加する要求を定義します。
ms.openlocfilehash: ca6850cfdc8a37bf0480db0c040b035591a59ce6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536374"
---
# <a name="createmanagedfolder"></a>CreateManagedFolder

**CreateManagedFolder 要素** は、管理されたカスタム フォルダーをメールボックスに追加する要求を定義します。 
  
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
|[FolderNames](foldernames.md) <br/> |メールボックスに追加する名前付き管理フォルダーの配列を格納します。  <br/> |
|[メールボックス](mailbox.md) <br/> |メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

要求を行うユーザーのアカウントには、管理フォルダーが作成されるメールボックスに対する FullAccess アクセス許可が必要です。 _-AccessRights _ パラメーターを Exchange管理シェル **Add-MailboxPermission** コマンドレットと一緒に使用して、FullAccess アクセス許可を割り当てできます。 
  
Exchange Web サービスを使用して管理フォルダーをメールボックスに追加することもできますが、Exchange Web Services を使用して使用可能な管理フォルダーの一覧にアクセスすることはできません。 使用可能な管理フォルダーの一覧を取得するには **、get-managedfolder** Exchangeコマンドレットを使用します。 **get-managedfolder** コマンドレットによって返されるリストには、管理されたカスタム フォルダーと管理された既定のフォルダーの両方が含まれます。 CreateManagedFolder 操作を使用して **メールボックスに追加できるのは、managedcustomfolder** 型のフォルダーのみです。 
  
> [!NOTE]
> Microsoft サーバーの DirectoryServices API を使用して管理フォルダーの一覧を取得.NET Framework。 
  
[FindFolder 操作を使用して、](findfolder-operation.md)メールボックス内の管理フォルダーを検索できます。 管理フォルダーは、要求で [BaseShape](baseshape.md) 要素を AllProperties に設定することで区別できます。 応答には、管理フォルダーとストア フォルダーを区別するための[ManagedFolderInformation](managedfolderinformation.md)要素Exchangeされます。 管理フォルダーは、他の種類のフォルダーを削除するのと同じ方法で削除できます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateManagedFolder 操作](createmanagedfolder-operation.md)
  
[FindFolder 操作](findfolder-operation.md)


[フォルダーの検索](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[管理フォルダーの追加](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

