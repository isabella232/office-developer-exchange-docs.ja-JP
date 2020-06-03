---
title: ExpandDL
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: affe84a5-ad98-4aba-83f4-8732938b763d
description: ExpandDL 要素は、配布リストを展開するための要求を定義します。
ms.openlocfilehash: 52b1ea1b51ce185c7a266e3002a4484e4b813bc0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456935"
---
# <a name="expanddl"></a>ExpandDL

**Expanddl**要素は、配布リストを展開するための要求を定義します。 
  
```xml
<ExpandDL>
   <Mailbox/>
</ExpandDL>
```

 **ExpandDLType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |完全に解決された電子メールアドレスまたは配布リストを識別します。 このメールボックスは、展開する配布リストを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

配布リストの展開は、1つの配布リストに対してのみ実行されます。 配布リストの展開が再帰的ではありません。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[ExpandDL 操作](expanddl-operation.md)

