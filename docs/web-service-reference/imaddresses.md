---
title: ImAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ImAddresses
api_type:
- schema
ms.assetid: 29f614a7-7fe6-47fa-b5f2-8feff106aa99
description: ImAddresses 要素は、連絡先のインスタント メッセージング アドレスのコレクションを表します。
ms.openlocfilehash: e8c7a22e8537a4526594042905f7bb8454238bf1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831861"
---
# <a name="imaddresses"></a>ImAddresses

**ImAddresses**要素は、連絡先のインスタント メッセージング アドレスのコレクションを表します。 
  
```xml
<ImAddresses>
   <Entry/>
</ImAddresses>
```

 **ImAddressDictionaryType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[エントリ (IMAddress)](entry-imaddress.md) <br/> |インスタント メッセージングの連絡先のアドレスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

