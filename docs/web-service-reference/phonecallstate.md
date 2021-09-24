---
title: PhoneCallState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: PhoneCallState 要素は、電話の現在の状態を指定します。
ms.openlocfilehash: 8c0b8357b58826f18f05eb0fedc0865be1623c2b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528303"
---
# <a name="phonecallstate"></a>PhoneCallState

**PhoneCallState** 要素は、電話の現在の状態を指定します。 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 **PhoneCallStateType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PhoneCallInformation](phonecallinformation.md) <br/> |電話の状態情報を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、PhoneCallState 要素に使用できる値を示** します。 
  
**PhoneCallState 要素の値**

|**値**|**説明**|
|:-----|:-----|
|アイドル状態  <br/> |初期呼び出しの状態。  <br/> |
|接続中  <br/> |システムは、この呼び出しをダイヤルしています。  <br/> |
|アラート  <br/> |通話がアラート状態です (電話が呼び出されています)。  <br/> |
|接続しました  <br/> |呼び出しは接続状態です。  <br/> |
|Disconnected  <br/> |呼び出しは切断されています。  <br/> |
|受信  <br/> |呼び出しは受信です。  <br/> |
|転送  <br/> |呼び出しが別の宛先に転送されています。  <br/> |
|転送  <br/> |呼び出しが別の宛先に転送されています。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの /ews/ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

