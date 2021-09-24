---
title: FolderName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderName
api_type:
- schema
ms.assetid: c5a2cd55-ac47-43bf-94b5-3ab3a4c28a62
description: FolderName 要素は、メールボックスに追加する 1 つの管理カスタム フォルダーを識別します。
ms.openlocfilehash: 76263d56c423411a58ea45d691ce93e2b3202571
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511566"
---
# <a name="foldername"></a>FolderName

**FolderName 要素は**、メールボックスに追加する 1 つの管理カスタム フォルダーを識別します。 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[FolderNames](foldernames.md)
  
[FolderName](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderNames](foldernames.md) <br/> |メールボックスに追加する名前付き管理カスタム フォルダーの配列を格納します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、フォルダー名を表します。
  
## <a name="remarks"></a>注釈

Exchange Web サービスを使用して管理カスタム フォルダーをメールボックスに追加することもできますが、同じテクノロジを使用して使用可能な管理カスタム フォルダーの一覧にアクセスすることはできません。 管理カスタム フォルダーの一覧は、Exchange 管理シェル コマンドを使用するか、Active Directory ディレクトリ サービスとインターフェイスする API を使用して取得できます。 フォルダー名は、対応する Active Directory オブジェクトの名前です。
  
[FindFolder 操作を使用して、](findfolder-operation.md)管理されたカスタム フォルダーを検索できます。 [DeleteFolder 操作を使用して、](deletefolder-operation.md)管理されたカスタム フォルダーを削除します。 
  
**FolderName** は組織内の既存の管理カスタム フォルダーの名前です。 組織に含めされていないフォルダーを追加しようとすると、エラー応答が発生します。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindFolder 操作](findfolder-operation.md)


[フォルダーの検索](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[管理フォルダーの追加](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

