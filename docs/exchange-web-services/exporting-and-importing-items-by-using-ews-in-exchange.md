---
title: Exchange で EWS を使用してアイテムをエクスポートおよびインポートする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ad5f75f9-47c3-4f51-a535-80cba4243683
description: Exchange の EWS マネージ API または EWS を使用して、予定、メール、連絡先、タスクなどのメールボックス アイテムをエクスポートおよびインポートする方法について説明します。
ms.openlocfilehash: 00c72806b95c162077733f77a52c4ea4da03631f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353652"
---
# <a name="exporting-and-importing-items-by-using-ews-in-exchange"></a>Exchange で EWS を使用してアイテムをエクスポートおよびインポートする

Exchange の EWS マネージ API または EWS を使用して、予定、メール、連絡先、タスクなどのメールボックス アイテムをエクスポートおよびインポートする方法について説明します。 
  
Exchange は重要な情報の宝庫で、メール、連絡先、タスク、予定表は組織の機能の中核をなします。 EWS を使用すると、3 つの異なるアプローチで中核となるアイテムの種類をエクスポートおよびインポートできます。
  
- アイテム の種類の交換。アイテムを他のシステムおよびファイルとの間でインポートおよびエクスポートする場合には、このアプローチの使用をお勧めします。
    
- アイテム レベルの機能 (EWS のみ)。1 つの Exchange サーバーまたはメールボックスからエクスポートまたはコピーし、別のものにインポートする場合にはこのシナリオをお勧めします。
    
- iCalendar や vCard などの一般的な標準ファイル形式の MIME ストリーム。プロパティ セットは限定的ですし MIME への変換はコストがかかるため、少量のデータのインポートまたはエクスポートの場合にのみこのアプローチをお勧めします。
    
> [!IMPORTANT]
> EWS は、メールボックスのバックアップと復元用には設計されていません。 データベースをバックアップして復元するには、「[バックアップと復元 API](../backup-restore/backup-and-restore-for-exchange-2013.md)」をご覧ください。 また、TechNet の「[バックアップ、復元、および障害回復](http://technet.microsoft.com/ja-JP/library/dd876874%28v=exchg.150%29.aspx)」もご覧ください。 
  
**表 1. 連絡先、メール、予定表アイテムのエクスポートおよびインポート**

|タスク|EWS マネージ API メソッド|EWS 操作|メモ|
|:-----|:-----|:-----|:-----|
|連絡先、メール、タスク、予定表アイテムのコピーを[プロパティ セットを指定して](properties-and-extended-properties-in-ews-in-exchange.md)エクスポートする。  <br/> |[Contact.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> [EmailMessage.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> [Appointment.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> [Task.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.task.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |メールボックス アイテムを Exchange 以外の別のシステムまたはファイル (vCard ファイル タイプと iCal ファイル タイプを含む) にエクスポートする場合には、このオプションをお勧めします。<br/>エクスポートされたプロパティ セットを制御できるため、また Exchange サーバーのパフォーマンスが良いため、通常はこれが最適なオプションです。<br/><br/>メールボックス アイテムのプロパティ セットによっては、およびアイテムに設定されているスキーマ化されていないプロパティ ID (拡張プロパティ) すべてにアプリケーションが対応しているかどうかによっては、このオプションでは、完全な再現性を持つコピーを生成できない場合があります。<br/><br/>これらのメソッドと操作は、アイテムのスキーマ化されたプロパティ セットと、要求された拡張プロパティを提供します。<br/>**Bind** メソッドまたは **GetItem** 操作でアイテムを完全な再現性を持つエクスポートを行えるのは、アイテムに設定されている拡張プロパティが分かっている場合のみです。<br/>すべての既知の[拡張プロパティ](properties-and-extended-properties-in-ews-in-exchange.md)を要求して、完全な再現性を有効にできます。<br/><br/>**ヒント**: EWS マネージ API のトレース機能を使用すると、エクスポートされたアイテムの XML 表現を取得できます。           詳しくは、「[カスタム形式にアイテムをエクスポートする](how-to-export-items-by-using-ews-in-exchange.md#bk_exportcustom)」をご覧ください。  <br/> |
|連絡先、メール、タスク、予定表アイテムのコピーを[プロパティ セットを指定して](properties-and-extended-properties-in-ews-in-exchange.md)インポートする。  <br/> |[Contact.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) <br/> [EmailMessage.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> [Appointment.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) <br/> [Task.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.task.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |Exchange にメールボックス アイテムをインポートする場合、このオプションをお勧めします。<br/>インポートされたアイテムの状態を維持するためにいくつかのアイテムの種類で特別なプロパティを設定しなければならない場合があります。<br/>一部のプロパティは Exchange によって設定されクライアントでは設定されないので、必ずしも完全に再現性のあるインポートとはなりません。<br/><br/>たとえば、出席者が含まれる会議をメールボックスにインポートすることはできません。Exchange が開催者と出席者との間に関係を設定しているためです。 <br/>この関係は、会議出席依頼を送信する開催者、およびそれを受け取って応答する出席者だけが設定できます。<br/><br/>Exchange の **Appointment** オブジェクトには複雑な関係を設定することができます。<br/> 出席者がいる予定 (会議) には、会議の開催者と出席者を結び付ける設定が含まれています。<br/>これらの設定は、予定をエクスポートおよびインポートするときに維持されません。<br/>会議の開催者/出席者の関係をプログラムによって予定に直接再設定することはできません。<br/>こうした関係を再設定するためのオプションとしては、インポート後に処理後のタスクを実行し、開催者が会議を再送信し、出席者がそれらの会議を承諾するようにします。<br/>Exchange の偽装を使用すると、開催者と出席者の両方に代わって呼び出しを行えます。<br/>会議がメールボックス内の他の会議に誤って関連付けられるという事態を避けるには、**Appointment** オブジェクトの UID プロパティを変更してからインポートする必要があります。  <br/> |
|連絡先、メール、タスク、予定表アイテムのコピーを完全な再現性でエクスポートする。  <br/> |適用できません  <br/> |[ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) <br/> |これは、Exchange メールボックスに再びインポートする予定のメールボックス アイテムをエクスポートするための最適なオプションです。<br/>このオプションを使用して、メールボックス間でアイテムをコピーすることもできます。<br/><br/>**ExportItems** 操作では、メールボックス間での情報の移動に使用できるアイテムを表す非透過ストリームが提供されます。<br/>**ExportItems** を [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) 操作と併用し、別のシステムでアイテムを検索するためのインデックスを作成できます。<br/>エクスポート ストリームを変更することはできません。  <br/> 詳しくは、「[完全な再現性でアイテムをエクスポートする](how-to-export-items-by-using-ews-in-exchange.md#bk_exportfullfidelity)」をご覧ください。  <br/> |
|連絡先、メール、タスク、予定表アイテムのコピーを完全な再現性でインポートする。  <br/> |適用できません  <br/> |[UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) <br/> |これは、**ExportItems** 操作でエクスポートされたアイテムをインポートするための唯一のオプションです。  <br/> |
|一般的なファイルの種類の連絡先、メール、予定表アイテムのコピーを MIME ストリームとしてエクスポートする。  <br/> |[Contact.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> [EmailMessage.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> [Appointment.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |**GetItem** <br/> |[MimeContent](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) プロパティを使用して、アイテムの MIME ストリーム表現を取得できます。<br/><br/>このストリームは、アイテムのすべてのプロパティの基本的なすべてのサブセットを提供します。<br/>1 回限りの操作ではこの MIME ストリームだけを使用するのがベスト プラクティスです。<br/>大規模で頻繁なアイテムのインポート/エクスポートでは MIME を使用しないでください。Exchange は MIME コンテンツの変換を実行するので、パフォーマンスに影響を及ぼす可能性があるためです。<br/><br/>**Contact** MIME ストリームは、[vCard](http://www.faqs.org/rfcs/rfc2426.html) (.vcf) ファイルです。<br/>連絡先に設定されているプロパティ セットによっては、完全な再現性のコピーが生成されない可能性があります。<br/>vCard MIME ストリームを使用して、連絡先をインポートすることはできません。<br/>詳しくは、「[vCard ファイルに連絡先をエクスポートする](how-to-export-items-by-using-ews-in-exchange.md#bk_exportvcardmime)」をご覧ください。<br/><br/>**EmailMessage** MIME ストリームは .eml ファイルです。<br/>.eml 形式は、Outlook およびその他のメール クライアントが識別できるので便利です。<br/>また、この MIME ストリームを使用して .mht ファイルを作成できますが、多くのブラウザーがこのファイルの種類を使用できるので便利です。<br/>EWS では、メールを .msg ファイルにエクスポートするための .msg ファイル ストリームは提供されません。<br/>.msg ファイルをエクスポートするには、**EmailMessage.Bind** メソッドの結果または **GetItem** 操作の呼び出し結果から [.MSG ファイルを構築](http://msdn.microsoft.com/ja-JP/library/cc463912%28v=EXCHG.80%29.aspx)するか、サード パーティ製 API を使用して EWS を呼び出した結果から .msg ファイルを構築します。<br/>詳しくは、「[.eml ファイルとしてメールをエクスポートする](how-to-export-items-by-using-ews-in-exchange.md#bk_exportemailmime)」をご覧ください。<br/><br/>**Appointment** MIME ストリームは iCal (.ics) ファイルです。<br/>.ics 形式は、Outlook およびその他のメール クライアントが識別できるものなので便利です。<br/>この MIME ストリームでは、出席者情報が提供されないため、会議をエクスポートするためにこのオプションを使用することはできません。 <br/>添付ファイルおよびその他のプロパティは、この MIME ストリームに含まれない可能性があります。<br/>iCal 形式を、[Appointment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトまたは **GetItem** 操作にで返される XML から構築することを検討してください。<br/>この方法を使用すると、iCal ファイルの拡張プロパティ (“X-‘ プロパティ) を含め、より多くの Exchange プロパティをキャプチャできます。<br/>また、XML 形式の予定をエクスポートすることもできます。<br/>**GetItem** 操作を呼び出して、システムに XML を保存します。<br/>また、EWS マネージ API の[トレース機能](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)を使用して、XML をキャプチャして XML データベースに格納できます。<br/>詳しくは、「[iCal ファイルとして予定をエクスポートする](how-to-export-items-by-using-ews-in-exchange.md#bk_exporticalmime)」をご覧ください。  <br/> |
|一般的なファイルの種類の MIME ストリームとしてメール、予定表アイテムのコピーをインポートする。  <br/> |[EmailMessage.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> [Appointment.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) <br/> |**CreateItem** <br/> |**EmailMessage** の **MimeContent** プロパティまたは **Appointment** オブジェクトを使用して .eml または .ics ファイルをインポートすることができます。<br/>メールが下書きではない場合、[PidTagMessageFlags (0x0E07)](http://msdn.microsoft.com/ja-JP/library/office/cc839733%28v=office.15%29.aspx) 拡張プロパティを設定する必要があります。<br/><br/>この方法で、会議をインポートすることはできません。  <br/> |
   
## <a name="alternatives-to-exporting-and-importing-items-by-using-ews"></a>EWS を使用したアイテムのエクスポートとインポート以外の方法
<a name="alternatives"> </a>

他の方法を使用して、Exporing メールボックスとの間でアイテムをインポート/エクスポートできます。インポートとエクスポートの戦略を設計するときに考慮できる事柄を次にいくつか示します。
  
- PowerShell を使用して EWS を呼び出し、出力を .csv ファイルに書式設定します。
    
- アイテムをエクスポートまたはインポートするには、MAPI を実装するサード パーティ ライブラリを使用します。EWS を .msg ファイルに変換することができるサード パーティ ライブラリも利用できます。
    
- Exchange 管理シェル、[MailboxImportRequest](http://technet.microsoft.com/ja-JP/library/ff607310%28v=exchg.150%29.aspx) コマンドレット、[MailboxExportRequest](http://technet.microsoft.com/ja-JP/library/ff607299%28v=exchg.150%29.aspx) コマンドレットを使用して、[メールボックスのインポートとエクスポートの要求を実行](http://technet.microsoft.com/ja-JP/library/ee633455%28v=exchg.150%29.aspx)します。 
    
- [Outlook のインポート オプション](http://office.microsoft.com/ja-JP/outlook-help/import-outlook-items-from-an-outlook-data-file-pst-HA102505743.aspx)を使用して、アイテムのインポートとエクスポートを行います。 
    
## <a name="in-this-section"></a>このセクションの内容
<a name="alternatives"> </a>

- [Exchange の EWS を使用してアイテムをエクスポートする](how-to-export-items-by-using-ews-in-exchange.md)    
- [Exchange の EWS を使用してアイテムをインポートする](how-to-import-items-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目

- [バックアップ、復元、および障害回復](http://technet.microsoft.com/ja-JP/library/dd876874%28v=exchg.150%29.aspx)  
- [ジャーナリング](http://technet.microsoft.com/ja-JP/library/aa998649%28v=exchg.150%29.aspx)    
- [Internet Calendaring and Scheduling Core Object Specification (RFC 5545)](http://tools.ietf.org/html/rfc5545)   
- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)
    

