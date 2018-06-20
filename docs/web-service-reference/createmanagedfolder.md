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
description: CreateManagedFolder 要素は、メールボックスに管理されたカスタム フォルダーを追加する要求を定義します。
ms.openlocfilehash: 4acc931de2a8665db092c3b309d914f0a3c67558
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759850"
---
# <a name="createmanagedfolder"></a>CreateManagedFolder

**CreateManagedFolder**要素は、メールボックスに管理されたカスタム フォルダーを追加する要求を定義します。 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 **CreateManagedFolderRequestType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[表示](foldernames.md) <br/> |メールボックスに追加するのには管理対象のフォルダーを名前付きの配列が含まれています。  <br/> |
|[メールボックス](mailbox.md) <br/> |メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

要求を行っているユーザーのアカウントによっては、メールボックスの管理フォルダーが作成される場所に FullAccess アクセス許可が必要です。 **追加 MailboxPermission**の Exchange 管理シェル コマンドレットで・ ・ アクセス権の _ _ パラメーターを使用するには FullAccess アクセス許可を割り当てるには。 
  
メールボックスに管理フォルダーを追加するのには、Exchange Web サービスを使用できますが、使用可能な管理対象フォルダーの一覧にアクセスするのには Exchange Web サービスを使うことはできません。 使用可能な管理対象フォルダーの一覧を取得するには、 **get managedfolder**の Exchange 管理シェル コマンドレットを使用します。 **Get managedfolder コマンドレット**によって返されるリストは、管理されたカスタム フォルダーおよび管理された既定フォルダーの両方に含まれます。 CreateManagedFolder オペレーションを使用してメールボックスにのみ型の**managedcustomfolder**のフォルダーを追加できます。 
  
> [!NOTE]
> 管理対象フォルダーの一覧は、Microsoft.NET Framework のつ API を使用しても取得できます。 
  
[FindFolder 操作](findfolder-operation.md)を使用すると、メールボックス内の管理フォルダーを検索します。 管理フォルダーは、要求に[BaseShape](baseshape.md)の要素を AllProperties に設定することで区別できます。 応答は、Exchange ストアのフォルダーから管理対象のフォルダーを識別するために[ManagedFolderInformation](managedfolderinformation.md)の要素に含まれます。 その他の種類のフォルダーを削除することと同じ方法で管理対象のフォルダーを削除できます。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateManagedFolder 操作](createmanagedfolder-operation.md)
  

  [FindFolder 操作](findfolder-operation.md)


[フォルダーを検索します。](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[管理フォルダーを追加します。](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

