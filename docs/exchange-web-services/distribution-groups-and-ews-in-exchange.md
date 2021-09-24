---
title: Exchange の配布グループと EWS
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: fe08c2e3-92a0-43ec-bc61-69b14caee8fe
description: Exchange で使用できる、さまざまな種類の配布グループと、それらを EWS マネージ API または EWS アプリケーションで管理する方法について説明します。
ms.openlocfilehash: 71dc1a1e4c71310943eb19f8a5d6b3f470ab7ccb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512304"
---
# <a name="distribution-groups-and-ews-in-exchange"></a>Exchange の配布グループと EWS

Exchange で使用できる、さまざまな種類の配布グループと、それらを EWS マネージ API または EWS アプリケーションで管理する方法について説明します。
  
配布グループは、1 つのエイリアスまたは電子メール アドレスに関連付けられている電子メール アドレスのコレクションです。配布グループ (配布リストとも呼ばれます) によって、ユーザーは 1 つの受信者アドレスを使用して複数のユーザーに電子メールを送信することができます。配布グループのメンバーシップのメッセージ受信者は個別の電子メール スレッドの外で管理できるため、配布グループはユーザーのグループへのメールの配信を有効にするための優れた方法を提供します。EWS マネージ API、EWS、および Exchange 管理シェルを使用することにより、プログラムを使用して配布グループを作成したり、管理することができます。プログラミングを開始する前に、使用可能な別の種類の配布グループと、それらを管理するためのオプションについて調べてみましょう。
  
## <a name="types-of-distribution-groups"></a>配布グループの種類

Exchange では、次の 3 種類の配布グループをサポートしています。
  
- [ユニバーサル配布グループ](distribution-groups-and-ews-in-exchange.md#bk_DistributionGroup) — メールが有効な Active Directory 配布グループ オブジェクト。ユニバーサル配布グループを使用すると、受信者のグループにメッセージを配布できます。 
    
- [セキュリティ グループ](distribution-groups-and-ews-in-exchange.md#bk_SecurityGroup) — メールが有効な Active Directory オブジェクト。ユニバーサル セキュリティ グループともいいます。 セキュリティ グループを使用すると、メッセージの配布だけでなく、Active Directory ドメイン サービス (AD DS) 内のリソースにアクセス許可を割り当てることができます。 
    
- [連絡先グループ](distribution-groups-and-ews-in-exchange.md#bk_ContactGroup) — ユーザーのメールボックス内にある非公開の配布グループ。 
    
選択する配布グループの種類は、配布グループの保存場所、使用するユーザー、使用する目的によって異なります。

<a name="bk_DistributionGroup"> </a>

### <a name="universal-distribution-groups"></a>ユニバーサル配布グループ

ユニバーサル配布グループを使用して、受信者のグループを 1 つのエイリアスまたは電子メール アドレスに統合できます。 ユニバーサル配布グループは AD DS に格納されているので、組織外のユーザーを含む、すべてのユーザーがこれらのグループを電子メールの送信に使用できます。 配布グループは EWS マネージ API または EWS を使用して展開できますが、配布グループの作成や管理には、[Exchange 管理シェル コマンドレット](#bk_UsingEMS)を使用する必要があります。
  
ユニバーサル配布グループを使用すると、たとえば会議室のコレクションを格納して、ユーザーが会議のための会議室を容易に見つけられるようにすることもできます。ユーザーは会議室の一覧 (会議室のリソース メールボックスを含むユニバーサル配布グループ) を会議出席依頼に追加して、使用可能な会議室を検索できます。各会議室を個別に追加する必要はありません。
  
メンバーシップを更新するまで同じ状態を維持する、静的なユニバーサル配布グループを作成できます。または、動的なユニバーサル配布グループを作成できます。動的なユニバーサル配布グループは Active Directory にメールが有効なオブジェクトを照会し、その結果に基づいてグループ メンバーシップを構築します。グループ メンバーシップは、グループに電子メール メッセージが送信されるたびに再計算されます。  

<a name="bk_SecurityGroup"> </a>

### <a name="security-groups"></a>セキュリティ グループ

ユニバーサル配布グループとセキュリティ グループは、ほとんどの点で同じです。ただし、ユニバーサル配布グループとは異なり、セキュリティ グループを使用すると AD DS 内のネットワーク リソースにアクセス許可を割り当てることができます。EWS マネージ API または EWS を使用してセキュリティ グループを作成および管理することはできません。代わりに [Exchange 管理シェル コマンドレット](#bk_UsingEMS) を使用してください。ただし、ユニバーサル配布グループと同様に、EWS マネージ API または EWS を使用してセキュリティ グループを展開することはできます。

<a name="bk_ContactGroup"> </a>

### <a name="contact-groups"></a>連絡先グループ

ユーザーごとにサーバーへの管理アクセス権を付与して配布グループを作成することは避けたいが、配布グループを有効にして 1 つのメッセージを大規模なユーザーのコレクションに送信したい場合は、連絡先グループを使用することで実現できます。 連絡先グループには、そのグループに関連付けられた電子メール アドレスがありません。また、連絡先グループは特定のユーザーのメールボックス内にのみ存在し、他のユーザーはそのグループにアクセスできません。 [EWS マネージ API または EWS を使用して連絡先グループを作成する](how-to-create-contact-groups-by-using-ews-in-exchange.md)ことができます。
  
## <a name="managing-distribution-groups-by-using-the-ews-managed-api-or-ews"></a>EWS マネージ API または EWS を使用した配布グループの管理

EWS マネージ API または EWS を使用すると、ユニバーサル配布グループやセキュリティ グループを展開したり、連絡先グループの作成および管理を制御できますが、これらのテクノロジを使用して、それらのグループのメンバーを作成したり、編集することはできません。 
  
**表 1. 配布グループを管理するための EWS マネージ API メソッドと EWS 操作**

|**EWS マネージ API メソッド**|**EWS 操作**|**使用目的**|
|:-----|:-----|:-----|
|[ContactGroup クラス](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx)のメソッド  <br/> |[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |Exchange ストアで連絡先グループを作成します。<br/><br/>**メモ**: EWS マネージ API または EWS を使用して、ユニバーサル配布グループやセキュリティ グループを作成することはできません。           |
|[ExpandGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) <br/> |[ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) <br/> |ユニバーサル配布グループ、セキュリティ グループ、または連絡先グループを、そのメンバーの一覧を取得することによって展開します。  <br/> |
|[FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |メールボックス内の連絡先グループを検索します。  <br/> |
|[GetRooms](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) <br/> |[GetRooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) <br/> |組織の指定された会議室の一覧にある、すべての会議室のコレクションを取得します。会議室の一覧は、会議室リソース メールボックスのみを格納する配布グループです。  <br/> |
|[ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |あいまいな名前に合致する可能性がある候補を検索し、それを返します。候補は配布グループになる可能性があります。  <br/> |
   
[ExpandGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) メソッドまたは [ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) 操作によって返される情報を使用して、グループ内のメンバーの種類を特定できます。 メンバーの種類は、[MailboxType](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.mailboxtype%28v=exchg.80%29.aspx) の EWS マネージ API 列挙体と、[MailboxType](https://msdn.microsoft.com/library/696e5fdb-d8c5-40f0-9e79-885eae65dfa4%28Office.15%29.aspx) の EWS 要素によって定義されます。 
  
**表 2. 配布グループのメンバーの種類**

|**MailboxType 列挙値**|**MailboxType 要素値**|**説明**|
|:-----|:-----|:-----|
|メールボックス  <br/> |メールボックス  <br/> |メールが有効な Active Directory オブジェクト。  <br/> |
|PublicGroup  <br/> |PublicDL  <br/> |展開したグループに含まれ配布グループ。メンバーの完全な一覧を取得するには、このグループも展開します。  <br/> |
|ContactGroup  <br/> |PrivateDL  <br/> |メールボックス内にある連絡先のグループ。そのメールボックスのユーザーにのみ使用できます。  <br/> |
|Contact  <br/> |Contact  <br/> |Exchange データベースの連絡先、または Active Directory のメール連絡先。  <br/> |

<a name="bk_UsingEMS"> </a>

## <a name="managing-distribution-groups-by-using-the-exchange-management-shell"></a>Exchange 管理シェルを使用した配布グループの管理

[Exchange 管理シェル コマンドレットを使用](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx)して、コード内にユニバーサル配布グループとセキュリティ グループを作成して管理できます。 
  
> [!NOTE]
> 連絡先グループの管理に Exchange 管理シェル コマンドレットは使用できません。 
  
**表 3. 配布グループを操作するための Exchange 管理シェル コマンドレット**

|**コマンドレット**|**使用目的**|
|:-----|:-----|
|[Disable-DistributionGroup](https://technet.microsoft.com/library/aa997942%28v=exchg.150%29.aspx) <br/> |メールが有効な配布グループからメール機能を削除します。  <br/> |
|[Enable-DistributionGroup](https://technet.microsoft.com/library/aa998916%28v=exchg.150%29.aspx) <br/> |既存のユニバーサル グループのメールを有効にします。  <br/> |
|[Get-DistributionGroup](https://technet.microsoft.com/library/bb124755%28v=exchg.150%29.aspx) <br/> |既存の配布グループを照会します。  <br/> |
|[New-DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx) <br/> |配布グループを作成します。  <br/> |
|[Remove-DistributionGroup](https://technet.microsoft.com/library/aa997627%28v=exchg.150%29.aspx) <br/> |AD DS から既存の配布グループを削除します。  <br/> |
|[Set-DistributionGroup](https://technet.microsoft.com/library/bb124955%28v=exchg.150%29.aspx) <br/> |既存の配布グループの設定を変更します。  <br/> |
|[Add-DistributionGroupMember](https://technet.microsoft.com/library/bb124340%28v=exchg.150%29.aspx) <br/> |配布グループに受信者を追加します。  <br/> |
|[Get-DistributionGroupMember](https://technet.microsoft.com/library/aa996367%28v=exchg.150%29.aspx) <br/> |既存の配布グループ メンバーを見つけます。  <br/> |
|[Remove-DistributionGroupMember](https://technet.microsoft.com/library/aa998016%28v=exchg.150%29.aspx) <br/> |配布グループから既存の受信者を削除します。  <br/> |
|[Update-DistributionGroupMember](https://technet.microsoft.com/library/dd335049%28v=exchg.150%29.aspx) <br/> |指定した配布グループのメンバーを更新します。  <br/> |
|[Get-DynamicDistributionGroup](https://technet.microsoft.com/library/bb124762%28v=exchg.150%29.aspx) <br/> |既存の動的配布グループの設定を取得します。  <br/> |
|[New-DynamicDistributionGroup](https://technet.microsoft.com/library/bb125127%28v=exchg.150%29.aspx) <br/> |動的配布グループを作成します。  <br/> |
|[Remove-DynamicDistributionGroup](https://technet.microsoft.com/library/bb125038%28v=exchg.150%29.aspx) <br/> |既存の動的配布グループを削除します。このコマンドレットは AD DS から動的配布グループを削除します。  <br/> |
|[Set-DynamicDistributionGroup](https://technet.microsoft.com/library/bb123796%28v=exchg.150%29.aspx) <br/> |既存の動的配布グループの設定を変更します。  <br/> |

<a name="bk_UsingEMS"> </a>

## <a name="in-this-section"></a>このセクションの内容

- [Exchange で EWS を使用して連絡先グループを作成する](how-to-create-contact-groups-by-using-ews-in-exchange.md)   
- [Exchange 2013 の EWS を使用して配布グループを展開する](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    
## <a name="see-also"></a>関連項目

- [Exchange 用の Web サービス クライアントの開発](develop-web-service-clients-for-exchange.md)   
- [マネージ コードからの Exchange 管理シェル コマンドレットの呼び出し](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx)
    

