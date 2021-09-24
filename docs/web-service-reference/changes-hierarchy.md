---
title: Changes (Hierarchy)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Changes
api_type:
- schema
ms.assetid: 918a0d1f-90a5-4eef-9592-07e15bef94e6
description: Changes 要素には、クライアント上のフォルダーと 2007 年 2007 年に実行されているコンピューター上のフォルダーの違いの種類を表す、変更の種類の配列がMicrosoft Exchange Serverされます。
ms.openlocfilehash: 1ecb43e37258ad5d8e12619436f14992cc2f788b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512122"
---
# <a name="changes-hierarchy"></a>Changes (Hierarchy)

**Changes** 要素には、クライアント上のフォルダーと 2007 年 2007 年に実行されているコンピューター上のフォルダーの違いの種類を表す、変更の種類の配列がMicrosoft Exchange Serverされます。 
  
[SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
  
[Changes (Hierarchy)](changes-hierarchy.md)
  
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
|[Create (FolderSync)](create-foldersync.md) <br/> |ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。  <br/> |
|[Update (FolderSync)](update-foldersync.md) <br/> |ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。  <br/> |
|[Delete (FolderSync)](delete-foldersync.md) <br/> |ローカル クライアント ストアで削除する 1 つのフォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |SyncFolderHierarchy 要求の状態と結果を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange 2007 コンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md)


[Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
  
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

