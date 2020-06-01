---
title: 変更 (階層)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Changes
api_type:
- schema
ms.assetid: 918a0d1f-90a5-4eef-9592-07e15bef94e6
description: Changes 要素には、クライアント上のフォルダーと、Microsoft Exchange Server 2007 を実行しているコンピューター上のフォルダーとの違いの種類を表す、変更の種類のシーケンス配列が含まれています。
ms.openlocfilehash: a296d87f23e85d42b4c8c858e92eddfb586a8324
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463273"
---
# <a name="changes-hierarchy"></a>変更 (階層)

**Changes**要素には、クライアント上のフォルダーと、Microsoft Exchange Server 2007 を実行しているコンピューター上のフォルダーとの違いの種類を表す、変更の種類のシーケンス配列が含まれています。 
  
[SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
  
[変更 (階層)](changes-hierarchy.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 **SyncFolderHierarchyChangesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Create (FolderSync)](create-foldersync.md) <br/> |ローカルクライアントストアに作成する1つのフォルダーを識別します。  <br/> |
|[Update (FolderSync)](update-foldersync.md) <br/> |ローカルクライアントストアで更新する1つのフォルダーを識別します。  <br/> |
|[Delete (FolderSync)](delete-foldersync.md) <br/> |ローカルクライアントストアで削除する1つのフォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |SyncFolderHierarchy 要求の状態と結果を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange 2007 コンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md)



  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
  
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

