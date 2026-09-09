---
layout: default
title: HushHours — Privacy Policy
---

# HushHours — Privacy Policy

**Last updated:** 2026-09-09

Languages: [English](#english) · [日本語](#japanese) · [한국어](#korean)

---

<a id="english"></a>

## English

### TL;DR

HushHours **does not collect, transmit, or share any data**. The app has no
internet permission, so it is technically incapable of sending anything
anywhere. Everything — including the content of blocked notifications — stays
on your device.

### 1. Information we collect

**None.** HushHours collects no personal information, usage data, telemetry,
crash reports, or analytics of any kind.

### 2. Information stored on your device

To do its job, HushHours stores the following locally, in its own private
app storage (a Room database and app preferences):

| Stored | Why |
|---|---|
| Your blocking rules — app package name, days, start and end times, blocking method | To know what to block and when. |
| Your keywords | To delete notifications containing words you chose. |
| Blocked notification history — the app it came from, the notification's title and text, the time, and the reason it was blocked | So you can check what was blocked while you were away. |
| Settings — language, theme, colour, defaults, history retention period | To remember your preferences. |

About the history: it does contain **notification text**, which can be
personal. Because of that:

- It is stored only on your device and is never transmitted.
- Cloud and device-to-device backup are disabled (`allowBackup="false"`), so it
  cannot leave the device that way either.
- Entries older than your chosen retention period (1, 3, 7 or 14 days;
  3 by default) are deleted automatically.
- You can delete history at any time from the History tab, or clear all app
  data / uninstall the app to remove everything.

### 3. Network usage

HushHours **does not declare the `INTERNET` permission**. Android itself
therefore blocks the app from opening any network connection. This is
verifiable from the app's manifest. There is no server, no account, and no
sign-in.

### 4. Permissions and why they are required

| Permission | Why |
|---|---|
| Notification access (`BIND_NOTIFICATION_LISTENER_SERVICE`) | The core of the app. Android grants it only when you enable it yourself in system settings. It is the only way an app can see a notification in order to block it. HushHours reads a notification's package name, title, text and category to decide whether one of your rules or keywords applies. Calls, alarms, media controls, navigation and emergency broadcasts are always let through. |
| Calendar (`READ_CALENDAR`) | Only for the optional "skip on public holidays" switch on a rule. The app looks for holiday events in the calendars already on your device. Nothing from your calendar is stored or sent, and the permission is requested only when you turn that switch on. |
| Notifications (`POST_NOTIFICATIONS`) | To post the single summary notification ("N blocked") at the end of a blocking window, when you choose the summary method. |
| Ignore battery optimizations (`REQUEST_IGNORE_BATTERY_OPTIMIZATIONS`) | To ask you to exempt the app, so the notification listener is not stopped in the background. Optional — the app works without it, less reliably. |
| Query installed apps (`<queries>`) | To list the apps that appear in your launcher, so you can pick which ones to block. The app deliberately does **not** use the broad `QUERY_ALL_PACKAGES` permission. The list is read locally and never leaves your device. |

### 5. Third-party services and SDKs

HushHours includes **no** third-party SDKs, ad networks, analytics, or crash
reporting libraries. Its only dependencies are AndroidX / Jetpack libraries
from Google (Compose, Room, Navigation) used for app structure. None of them
transmit user data.

### 6. Backup files you create yourself

The app can export your rules and keywords to a JSON file of your choosing,
through the Android file picker. That file is created and read only where you
put it, and its contents are your rules and keywords — no notification history
is included. What happens to a file after you export it is up to you.

### 7. Children's privacy

HushHours is not directed at children under 13. The app knowingly collects no
data from anyone, including children.

### 8. Changes to this policy

This policy may be updated as the app evolves. Updates are reflected by
changing the "Last updated" date at the top of this page.

### 9. Contact

[contact@13each.com](mailto:contact@13each.com)

---

<a id="japanese"></a>

## 日本語

### 要約

HushHours は**データの収集・送信・共有を一切行いません**。インターネット権限を
持たないため、仕組みとして外部に送ることができません。ブロックした通知の内容を
含め、すべて端末の中だけに残ります。

### 1. 収集する情報

**ありません。** 個人情報、利用状況、テレメトリ、クラッシュレポート、解析データの
いずれも収集しません。

### 2. 端末内に保存される情報

機能のために、次のものをアプリ専用の保存領域(Room データベースとアプリ設定)に
保存します。

| 保存するもの | 目的 |
|---|---|
| ブロックのルール — アプリのパッケージ名、曜日、開始・終了時刻、ブロック方法 | 何をいつブロックするかの判定に使います。 |
| キーワード | 指定した単語を含む通知を削除するために使います。 |
| ブロック履歴 — 送信元アプリ、通知のタイトルと本文、時刻、ブロックの理由 | 席を外している間に何がブロックされたかを確認できるようにするためです。 |
| 設定 — 言語、テーマ、色、新規ルールの初期値、履歴の保存期間 | 設定を覚えておくためです。 |

履歴には**通知の本文が含まれます**。個人的な内容になり得るため、次のように
扱っています。

- 端末内にのみ保存し、外部には一切送信しません。
- クラウドバックアップと端末間の引き継ぎを無効化しています(`allowBackup="false"`)。
  そのためバックアップ経由でも端末の外に出ません。
- 選んだ保存期間(1・3・7・14日、既定は3日)を過ぎた記録は自動で削除されます。
- 履歴タブからいつでも削除できます。アプリのデータ削除、またはアンインストールで
  すべて消えます。

### 3. ネットワークの利用

HushHours は **`INTERNET` 権限を宣言していません**。したがって Android 自体が
このアプリのネットワーク接続を禁止します。これはアプリのマニフェストから確認
できます。サーバーもアカウントもログインもありません。

### 4. 権限とその理由

| 権限 | 理由 |
|---|---|
| 通知へのアクセス(`BIND_NOTIFICATION_LISTENER_SERVICE`) | このアプリの中核です。ご自身がシステム設定で許可したときにのみ Android が付与します。通知をブロックするには、まずアプリが通知を見られる必要があり、その手段はこれだけです。ルールやキーワードに当たるかを判定するため、通知のパッケージ名・タイトル・本文・カテゴリを読みます。通話、アラーム、メディア操作、ナビ、緊急放送は常に通します。 |
| カレンダー(`READ_CALENDAR`) | ルールの任意設定「祝日はブロックしない」のためだけに使います。端末に既にあるカレンダーの祝日予定を探します。カレンダーの内容を保存・送信することはなく、この設定をオンにするときにだけ権限を要求します。 |
| 通知(`POST_NOTIFICATIONS`) | ブロック方法に「要約」を選んだとき、時間帯の終わりに要約通知(「N件ブロック」)を1件送るために使います。 |
| 電池最適化の除外(`REQUEST_IGNORE_BATTERY_OPTIMIZATIONS`) | 通知リスナーがバックグラウンドで停止されないよう、除外の許可をお願いするために使います。任意です — なくても動作しますが、安定性は落ちます。 |
| インストール済みアプリの照会(`<queries>`) | ランチャーに表示されるアプリを一覧し、ブロック対象を選べるようにするためです。範囲の広い `QUERY_ALL_PACKAGES` 権限は**意図的に使っていません**。一覧は端末内で読むだけで、外に出ることはありません。 |

### 5. 第三者のサービス・SDK

第三者の SDK、広告ネットワーク、解析、クラッシュレポートのライブラリは**一切
含みません**。依存しているのはアプリの構造に使う Google の AndroidX / Jetpack
ライブラリ(Compose、Room、Navigation)のみで、いずれもユーザーデータを送信
しません。

### 6. ご自身が作成するバックアップファイル

ルールとキーワードを、Android のファイル選択画面で指定した場所に JSON ファイル
として書き出せます。ファイルは指定した場所にのみ作成・読み込みされ、内容は
ルールとキーワードです — **ブロック履歴は含みません**。書き出したファイルの
その後の取り扱いはご自身の管理となります。

### 7. 子どものプライバシー

HushHours は13歳未満の子どもを対象としていません。子どもを含め、誰からも
データを収集しません。

### 8. 本方針の変更

アプリの変更に合わせて本方針を更新する場合があります。更新はページ上部の
「Last updated」の日付で示します。

### 9. お問い合わせ

[contact@13each.com](mailto:contact@13each.com)

---

<a id="korean"></a>

## 한국어

### 요약

HushHours는 **어떤 데이터도 수집·전송·공유하지 않습니다.** 인터넷 권한이 없어
구조적으로 외부에 보낼 수 없습니다. 차단된 알림의 내용까지 포함해 모든 것이
기기 안에만 남습니다.

### 1. 수집하는 정보

**없습니다.** 개인정보, 사용 기록, 텔레메트리, 크래시 리포트, 분석 데이터 중
어떤 것도 수집하지 않습니다.

### 2. 기기에 저장되는 정보

기능을 위해 아래 항목을 앱 전용 저장 영역(Room 데이터베이스와 앱 설정)에
저장합니다.

| 저장 항목 | 목적 |
|---|---|
| 차단 규칙 — 앱 패키지명, 요일, 시작·종료 시각, 차단 방식 | 무엇을 언제 차단할지 판단합니다. |
| 키워드 | 지정한 단어가 포함된 알림을 삭제합니다. |
| 차단 히스토리 — 보낸 앱, 알림의 제목과 본문, 시각, 차단 사유 | 자리를 비운 사이 무엇이 차단됐는지 확인할 수 있게 합니다. |
| 설정 — 언어, 테마, 색상, 새 규칙 기본값, 히스토리 보관 기간 | 선택한 설정을 기억합니다. |

히스토리에는 **알림 본문이 포함됩니다.** 개인적인 내용일 수 있어 다음과 같이
다룹니다.

- 기기 안에만 저장하며 외부로 전송하지 않습니다.
- 클라우드 백업과 기기 간 이전을 비활성화했습니다(`allowBackup="false"`).
  백업 경로로도 기기를 벗어나지 않습니다.
- 선택한 보관 기간(1·3·7·14일, 기본 3일)이 지난 기록은 자동 삭제됩니다.
- 히스토리 탭에서 언제든 삭제할 수 있고, 앱 데이터 삭제나 앱 제거로 전부
  없어집니다.

### 3. 네트워크 사용

HushHours는 **`INTERNET` 권한을 선언하지 않습니다.** 따라서 Android가 이 앱의
네트워크 연결 자체를 막습니다. 앱 매니페스트에서 확인할 수 있습니다. 서버도,
계정도, 로그인도 없습니다.

### 4. 권한과 필요한 이유

| 권한 | 이유 |
|---|---|
| 알림 접근(`BIND_NOTIFICATION_LISTENER_SERVICE`) | 앱의 핵심입니다. 사용자가 시스템 설정에서 직접 허용할 때만 Android가 부여합니다. 알림을 차단하려면 먼저 앱이 알림을 볼 수 있어야 하고, 그 방법은 이것뿐입니다. 규칙이나 키워드에 해당하는지 판단하기 위해 알림의 패키지명·제목·본문·카테고리를 읽습니다. 전화, 알람, 미디어 컨트롤, 내비게이션, 재난 방송은 항상 통과시킵니다. |
| 캘린더(`READ_CALENDAR`) | 규칙의 선택 옵션인 "공휴일에는 차단하지 않기"에만 사용합니다. 기기에 이미 있는 캘린더에서 공휴일 일정을 찾습니다. 캘린더 내용을 저장하거나 전송하지 않으며, 이 옵션을 켤 때만 권한을 요청합니다. |
| 알림(`POST_NOTIFICATIONS`) | 차단 방식으로 "요약"을 선택했을 때, 시간대가 끝나는 시점에 요약 알림("N건 차단") 1건을 보내기 위해 사용합니다. |
| 배터리 최적화 제외(`REQUEST_IGNORE_BATTERY_OPTIMIZATIONS`) | 알림 리스너가 백그라운드에서 중단되지 않도록 제외를 요청하기 위해 사용합니다. 선택 사항입니다 — 없어도 동작하지만 안정성이 떨어집니다. |
| 설치된 앱 조회(`<queries>`) | 런처에 표시되는 앱을 나열해 차단 대상을 고를 수 있게 합니다. 범위가 넓은 `QUERY_ALL_PACKAGES` 권한은 **의도적으로 사용하지 않습니다.** 목록은 기기 안에서만 읽고 외부로 나가지 않습니다. |

### 5. 제3자 서비스 및 SDK

제3자 SDK, 광고 네트워크, 분석, 크래시 리포트 라이브러리를 **전혀 포함하지
않습니다.** 의존성은 앱 구조에 쓰는 Google의 AndroidX / Jetpack 라이브러리
(Compose, Room, Navigation)뿐이며 어느 것도 사용자 데이터를 전송하지 않습니다.

### 6. 사용자가 직접 만드는 백업 파일

규칙과 키워드를 Android 파일 선택 화면에서 지정한 위치에 JSON 파일로 내보낼 수
있습니다. 파일은 지정한 위치에만 만들어지고 읽히며, 내용은 규칙과 키워드입니다
— **차단 히스토리는 포함되지 않습니다.** 내보낸 파일의 이후 관리는 사용자
책임입니다.

### 7. 아동의 개인정보

HushHours는 13세 미만 아동을 대상으로 하지 않습니다. 아동을 포함해 누구로부터도
데이터를 수집하지 않습니다.

### 8. 본 방침의 변경

앱이 변경되면 본 방침도 갱신될 수 있습니다. 갱신은 페이지 상단의
"Last updated" 날짜로 표시합니다.

### 9. 문의

[contact@13each.com](mailto:contact@13each.com)
