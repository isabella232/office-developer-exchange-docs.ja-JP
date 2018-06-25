---
title: Exchange で EWS を使用してアイテムをエクスポートおよびインポートする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ad5f75f9-47c3-4f51-a535-80cba4243683
description: 'Exchange の EWS マネージ API または EWS を使用して、予定、メール、連絡先、タスクなどのメールボックス アイテムをエクスポートおよびインポートする方法について説明します。 '
ms.openlocfilehash: 63ba8807dd63ca2d151b1c2b1277625daeed640c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758909"
---
# <a name="exporting-and-importing-items-by-using-ews-in-exchange"></a>Exchange で EWS を使用してアイテムをエクスポートおよびインポートする

Exchange の EWS マネージ API または EWS を使用して、予定、メール、連絡先、タスクなどのメールボックス アイテムをエクスポートおよびインポートする方法について説明します。  
  
Exchange は、多くの重要な情報: 電子メール、連絡先、タスク、およびカレンダーは、組織の機能の中核です。 EWS を使用すると、エクスポートおよびインポートの 3 つの異なるアプローチを使用して主要な項目の種類。
  
- Exchange アイテムの種類。アイテムを他のシステムおよびファイルとの間でインポートおよびエクスポートする場合には、このアプローチの使用をお勧めします。
    
- アイテム レベルの機能 (EWS のみ)。1 つの Exchange サーバーまたはメールボックスからエクスポートまたはコピーし、別のものにインポートする場合にはこのシナリオをお勧めします。
    
- iCalendar や vCard などの一般的な標準ファイル形式の MIME ストリーム。プロパティ セットは限定的ですし MIME への変換はコストがかかるため、少量のデータのインポートまたはエクスポートの場合にのみこのアプローチをお勧めします。
    
> [!IMPORTANT]
> EWS では、メールボックスのバックアップと復元の設計されていません。 バックアップおよび復元するデータベースを[バックアップおよび復元の API](../backup-restore/backup-and-restore-for-exchange-2013.md)を使用します。 TechNet では[バックアップ、リストア、災害復旧](http://technet.microsoft.com/en-us/library/dd876874%28v=exchg.150%29.aspx)も参照してください。 
  
**表 1 です。エクスポートして、連絡先、電子メール、および予定表アイテムをインポートします。**

|**タスク**|**EWS マネージ API メソッド**|**EWS 操作**|**メモ**|
|:-----|:-----|:-----|:-----|
|連絡先、電子メール、タスク、または[指定したプロパティの設定](properties-and-extended-properties-in-ews-in-exchange.md)の予定表アイテムのコピーをエクスポートします。  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> [Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> [Task.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |メールボックス アイテムを Exchange 以外の別のシステムまたはファイル (vCard ファイル タイプと iCal ファイル タイプを含む) にエクスポートする場合には、このオプションをお勧めします。エクスポートされたプロパティ セットを制御できるため、また Exchange サーバーのパフォーマンスが良いため、通常はこれが最適なオプションです。<br/> メールボックス アイテムのプロパティ セットによっては、およびアイテムに設定されているスキーマ化されていないプロパティ ID (拡張プロパティ) すべてにアプリケーションが対応しているかどうかによっては、このオプションでは、完全な再現性を持つコピーを生成できない場合があります。  <br/> これらの方法と操作は、アイテムのプロパティと、要求された拡張プロパティのスキーマのセットを提供します。 **Bind**メソッドまたは**GetItem**操作だけできる項目の完全なエクスポート アイテムに設定されている拡張プロパティがわかっている場合。 忠実を有効にするのにはのすべての既知[の拡張プロパティ](properties-and-extended-properties-in-ews-in-exchange.md)を要求することができます。  <br/> > [!TIP]> EWS のマネージ API でトレース機能を使用すると、エクスポートされたアイテムの XML 表現を取得するのにすることができます。           詳細については、[カスタム形式にアイテムをエクスポートする](how-to-export-items-by-using-ews-in-exchange.md#bk_exportcustom)を参照してください。  <br/> |
|連絡先、電子メール、タスク、または[指定したプロパティの設定](properties-and-extended-properties-in-ews-in-exchange.md)の予定表アイテムのコピーをインポートします。  <br/> |[Contact.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) <br/> [EmailMessage.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> [Appointment.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) <br/> [Task.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |Exchange にメールボックス アイテムをインポートする場合、このオプションをお勧めします。インポートされたアイテムの状態を維持するためにいくつかのアイテムの種類で特別なプロパティを設定しなければならない場合があります。一部のプロパティは Exchange によって設定されクライアントでは設定されないので、必ずしも完全に再現性のあるインポートとはなりません。<br/> たとえば、出席者が含まれる会議をメールボックスにインポートすることはできません。Exchange が開催者と出席者との間に関係を設定しているためです。この関係は、会議出席依頼を送信する開催者、およびそれを受け取って応答する出席者だけが設定できます。<br/> **予定**オブジェクトを Exchange では、複雑な関係と設定を持つことができます。 (会議) の出席者の予定には、会議の開催者と出席者の会議を結合する設定があります。 エクスポートの予定をインポートすると、これらの設定は維持されません。 会議の開催者と出席者の関係上で直接プログラムを使用して再同期、予定はサポートされません。 オプションを実行するのには、これらの関係を再確立するが次の会議を再送信して、出席者が会議を承諾する会議の開催者にある、インポート後の後処理します。 Exchange の偽装を使用すると、開催者と出席者の両方の呼び出しを行います。 正しく、メールボックス内の他の会議に関連する会議のことを避けるためにインポートする前に**予定**オブジェクトの UID プロパティを変更する必要があります。  <br/> |
|連絡先、メール、タスク、予定表アイテムのコピーを完全な再現性でエクスポートする  <br/> |適用できません  <br/> |[ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) <br/> |これは、Exchange メールボックスにインポートするメールボックスのアイテムをエクスポートするための最適なオプションです。 メールボックスの間でアイテムをコピーするのにはこのオプションを使用することもできます。 **ExportItems**操作は、メールボックスとの間の情報の移動に使用できるアイテムを表す非透過のストリームを提供します。 [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)操作で**ExportItems**を使用すると、別のシステムで項目を検索するインデックスを作成します。 エクスポートのストリームを変更することはできません。  <br/> 詳細については、[完全な忠実性を持つアイテムをエクスポートする](how-to-export-items-by-using-ews-in-exchange.md#bk_exportfullfidelity)を参照してください。  <br/> |
|連絡先、メール、タスク、予定表アイテムのコピーを完全な再現性でインポートする   <br/> |適用できません  <br/> |[UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) <br/> |これは、 **ExportItems**操作によってエクスポートされたアイテムをインポートするための唯一のオプションです。  <br/> |
|一般的なファイルの種類の連絡先、メール、予定表アイテムのコピーを MIME ストリームとしてエクスポートする   <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> [Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |**GetItem** <br/> |[MimeContent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx)プロパティを使用するには、MIME ストリーム形式の項目を取得します。  <br/> このストリームは、アイテムのすべてのプロパティの基本的なすべてのサブセットを提供します。1 回限りの操作ではこの MIME ストリームだけを使用するのがベスト プラクティスです。大規模で頻繁なアイテムのインポート/エクスポートでは MIME を使用しないでください。Exchange は MIME コンテンツの変換を実行するので、パフォーマンスに影響を及ぶ可能性があるためです。<br/> **連絡先**の MIME ストリームは、 [vCard](http://www.faqs.org/rfcs/rfc2426.mdl) (.vcf) ファイルです。 連絡先に設定されているプロパティ、に応じてこの可能性があります完全なコピーを作成できません。 VCard の MIME ストリームを使用して連絡先をインポートすることはできませんに注意してください。 詳細については、 [vCard ファイルに連絡先をエクスポートする](how-to-export-items-by-using-ews-in-exchange.md#bk_exportvcardmime)を参照してください。  <br/> **Email メッセージ**の MIME ストリームは、.eml ファイルです。 .Eml 形式は、Outlook およびその他の電子メール クライアントはこれで識別できるため便利です。 多くのブラウザーはそのファイルの種類を使用できますので便利ですが、.mht ファイルを作成するのには、MIME ストリームを使用することもできます。 EWS では、.msg ファイルに電子メールをエクスポートするため、.msg ファイルのストリームを提供していません。 .Msg ファイルをエクスポートするためのオプションは、どちらかに[のコンス トラクターにします。MSG ファイルを](http://msdn.microsoft.com/en-us/library/cc463912%28v=EXCHG.80%29.aspx)、 **EmailMessage.Bind**メソッドまたは**GetItem**操作の結果から [呼び出し]、または EWS を呼び出すし、結果からの .msg ファイルを構築するサード ・ パーティ製の API を使用します。 詳細については、 [.eml ファイルとして電子メールのエクスポート](how-to-export-items-by-using-ews-in-exchange.md#bk_exportemailmime)を参照してください。  <br/> **予定**の MIME ストリームは、iCal (.ics) ファイルです。 .Ics 形式は、Outlook およびその他の電子メール クライアントはこれで識別できるため便利です。 MIME ストリームには、出席者情報は明記されていないために、会議をエクスポートするための実行可能なオプションではありません。 添付ファイルおよびその他のプロパティは、MIME ストリームに含まれません可能性があります。 [予定](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)オブジェクトとは、 **GetItem**操作によって返された XML から iCal 形式を作成することを検討してください。 この方法では、キャプチャすることも複数の拡張プロパティを使用して Exchange プロパティ ("x ' プロパティ) iCal ファイルにします。 XML 形式の予定をエクスポートすることもできます。 **GetItem**操作を呼び出すし、システムに XML を保存します。 XML データベースに格納するのに XML を取得するのには、EWS のマネージ API で[トレース機能](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)を使用することもできます。 詳細については、 [iCal ファイルとして予定をエクスポートする](how-to-export-items-by-using-ews-in-exchange.md#bk_exporticalmime)を参照してください。  <br/> |
|一般的なファイルの種類の MIME ストリームとしてメール、予定表アイテムのコピーをインポートする  <br/> |[EmailMessage.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> [Appointment.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) <br/> |**CreateItem** <br/> |**Email メッセージ**や**予定**オブジェクトの**MimeContent**プロパティを使用して、.eml ファイルまたは .ics ファイルをインポートできます。 [PidTagMessageFlags (0x0E07)](http://msdn.microsoft.com/en-us/library/office/cc839733%28v=office.15%29.aspx)の電子メールが、下書きではない場合、拡張プロパティを設定する必要があります。  <br/> この方法で、会議をインポートすることはできません。  <br/> |
   
## <a name="alternatives-to-exporting-and-importing-items-by-using-ews"></a>EWS を使用したアイテムのエクスポートとインポート以外の方法
<a name="alternatives"> </a>

他の方法を使用して、Exporing メールボックスとの間でアイテムをインポート/エクスポートできます。インポートとエクスポートの戦略を設計するときに考慮できる事柄を次にいくつか示します。
  
- PowerShell を使用して EWS を呼び出し、出力を .csv ファイルに書式設定します。
    
- MAPI を実装するサード パーティ製のライブラリを使用して、アイテムのエクスポート/インポートを行います。また、EWS を .msg ファイルに変換するサード パーティ製ライブラリも利用できます。
    
- [メールボックスのインポートを実行し要求をエクスポート](http://technet.microsoft.com/en-us/library/ee633455%28v=exchg.150%29.aspx)する Exchange 管理シェルと[MailboxImportRequest](http://technet.microsoft.com/en-us/library/ff607310%28v=exchg.150%29.aspx)と[MailboxExportRequest](http://technet.microsoft.com/en-us/library/ff607299%28v=exchg.150%29.aspx)コマンドレットを使用します。 
    
- インポートおよびエクスポートするアイテムを[Outlook のインポートのオプション](http://office.microsoft.com/en-us/outlook-help/import-outlook-items-from-an-outlook-data-file-pst-HA102505743.aspx)を使用します。 
    
## <a name="in-this-section"></a>このセクションの内容
<a name="alternatives"> </a>

- [Exchange EWS を使用して項目をエクスポートします。](how-to-export-items-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用してアイテムをインポート](how-to-import-items-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目


- [バックアップ、復元、および災害復旧](http://technet.microsoft.com/en-us/library/dd876874%28v=exchg.150%29.aspx)
    
- [ジャーナル処理](http://technet.microsoft.com/en-us/library/aa998649%28v=exchg.150%29.aspx)
    
- [インターネット予定表とスケジュールの中核となるオブジェクトの仕様 (RFC 5545)](http://tools.ietf.org/html/rfc5545)
    
- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)
    

