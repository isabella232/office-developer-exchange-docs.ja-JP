---
title: ChildFolderCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ChildFolderCount
api_type:
- schema
ms.assetid: e0e4eabd-802f-4dd0-9911-89e08c66a15e
description: ChildFolderCount 要素は、フォルダー内に含まれる直接の子フォルダーの数を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。
ms.openlocfilehash: c05d93e3f9df2d2acbb1b65f1116dab1aea24a3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537002"
---
# <a name="childfoldercount"></a>ChildFolderCount

**ChildFolderCount** 要素は、フォルダー内に含まれる直接の子フォルダーの数を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 
  
```xml
<ChildFolderCount/>
```

 **int**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |メールボックス内のフォルダーを表します。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |メールボックス内の予定表フォルダーを表します。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックス内の連絡先フォルダーを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックス内の検索フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスク フォルダーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は整数を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

