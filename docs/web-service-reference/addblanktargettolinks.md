---
title: Add空白 Targettolインク
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: AddBlankTargetToLinks 要素は、HTML リンクの target 属性が新しいウィンドウを開くように設定されていることを示します。
ms.openlocfilehash: 1d4d36c1f4b98ebee96baea683c40527d2a9ec27
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465044"
---
# <a name="addblanktargettolinks"></a>Add空白 Targettolインク

**Addblanktargettolinks**要素は、HTML リンクの target 属性が新しいウィンドウを開くように設定されていることを示します。 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

**xs: Boolean**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | **GetItem**、 **FindItem**、 **GetConversationItems** 、または**syncfolderitems**応答に含めるアイテムのプロパティとコンテンツを識別します。<br/><br/>  この要素の XPath 式は次のとおりです。<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a>テキスト値

**Addblanktargettolinks**要素のテキスト値が**true の場合**は、すべての HTML リンクが新しいウィンドウを開くように設定されていることを示します。 **False**を指定すると、現在のウィンドウで HTML リンクが開きます。 
  
## <a name="remarks"></a>注釈

この要素は省略できます。
  
この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

