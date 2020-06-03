---
title: Maxの戻り値
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxChangesReturned
api_type:
- schema
ms.assetid: f471db84-a666-4dfa-9993-8ca9113a0384
description: Maxchanges 返される要素は、同期応答で返すことができる変更の最大数を示します。
ms.openlocfilehash: caf96b6e95f2e63d0e544ead26fbea18cd637861
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460086"
---
# <a name="maxchangesreturned"></a>Maxの戻り値

**Maxchanges 返さ**れる要素は、同期応答で返すことができる変更の最大数を示します。 
  
[SyncFolderItems](syncfolderitems.md)
  
[Maxの戻り値](maxchangesreturned.md)
  
```xml
<MaxChangesReturned/>
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
|[SyncFolderItems](syncfolderitems.md) <br/> |Exchange ストアフォルダー内のアイテムを同期する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、単一の同期呼び出しで返されるアイテムの最大数を示す整数を表します。 この値は、1 ~ 512 の範囲にする必要があります。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderItems 操作](syncfolderitems-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

