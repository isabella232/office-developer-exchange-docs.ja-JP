---
title: Exchange の EWS での委任に関連するエラーの処理
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 631d364f-e324-4838-a92c-820286f771f8
description: Exchange の EWS マネージ API または EWS を使用して開発したアプリケーションの委任に関連するエラーを処理する方法を確認します。
ms.openlocfilehash: 3851709888e3a1087df02eea5d4d58888ad168e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758890"
---
# <a name="handling-delegation-related-errors-in-ews-in-exchange"></a>Exchange の EWS での委任に関連するエラーの処理

Exchange の EWS マネージ API または EWS を使用して開発したアプリケーションの委任に関連するエラーを処理する方法を確認します。
  
アプリケーションでは、委任を使用して、追加またはまたはデリゲートを削除、する場合、委任に関連するエラーを処理する必要があります。 または、EWS アプリケーションを開発するとき、実行時にこれらのエラーを処理することができます。 これらのエラーは、EWS のマネージ API[サービス エラー](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx)の列挙体と、EWS の[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素によって定義されます。 
  
## <a name="delegation-related-errors"></a>委任に関連するエラー

|**Error**|**しようとするときに発生しています.**|**処理方法**|
|:-----|:-----|:-----|
|ErrorItemNotFound  <br/> ErrorFolderNotFound  <br/> |アクセス権のないメールボックス、フォルダー、またはアイテムで操作を実行するとき。  <br/> |[UpdateDelegates](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) EWS のマネージ API のメソッド、EWS の[UpdateDelegate](http://msdn.microsoft.com/library/03f618ac-ad1a-4772-9b81-c5bb0f12d6ab%28Office.15%29.aspx) 、または操作を呼び出すと、要求を再試行して、フォルダーまたはアイテムのアクセスを有効にする代理人のアクセス許可を更新しています。  <br/> |
|ErrorAccessDenied  <br/> |変更を行う十分な権限が自分にないアイテムを変更するとき。  <br/> |**UpdateDelegate** EWS のマネージ API のメソッド、EWS の**UpdateDelegate** 、または操作を呼び出すと、要求を再試行して、[代理アクセス権を更新しています。  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |メールボックスの所有者をメールボックスの代理人として追加しようとするとき。  <br/> |[代理人として別のユーザーを追加する](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)メールボックスの所有者ではありません。  <br/> |
|ErrorDelegateAlreadyExists  <br/> |代理人が既に存在する場合に代理人を追加するとき。  <br/> |メールボックス所有者の代理人が既に存在するため、何も行われない。 または、既存のデリゲートのアクセス許可を変更しようとしている場合を使用して、 **UpdateDelegates**メソッドまたは**UpdateDelegate**操作します。  <br/> |
|ErrorNotDelegate  <br/> |メールボックスの代理アクセス許可を持たないユーザーの代理アクセス許可を変更するとき。  <br/> |[代理人としてユーザーを追加する](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)前に、メールボックスの更新または削除のアクセス許可。  <br/> |
|ErrorDelegateNoUser  <br/> |Active Directory ドメイン サービス (AD DS) ではないユーザーに代理アクセス権を変更します。  <br/> |、AD DS でユーザーを作成するか、依頼の代理人の情報を修正します。  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |代理人を使用して、メールボックスの所有者の代理として通知をサブスクライブするとき。  <br/> |メールボックスの所有者として通知をサブスクライブします。  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |プリンシパルのメールボックス サーバーとは異なるサーバーのバージョンを持つ代理人からの要求を作成するとき。  <br/> |代理人を使用するか、メールボックスがメールボックスの所有者と同じサーバーのバージョンの代理人を追加します。  <br/> |
|ErrorMissingEmailAddress  <br/> |メールボックスを持たない代理人アカウントを使用して要求を作成するとき。  <br/> |代理人のアカウントにメールボックスを追加します。  <br/> |
   
## <a name="see-also"></a>関連項目


- [Exchange での代理人アクセスと EWS](delegate-access-and-ews-in-exchange.md)
    
- [Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

