---
layout: default
title: Battery Charm — Privacy Policy
---

# Battery Charm — Privacy Policy

**Last updated:** 2026-11-05

Languages: [English](#english) · [日本語](#japanese) · [한국어](#korean)

---

<a id="english"></a>

## English

### TL;DR

Battery Charm **does not collect, sell, or share any personal data**. The app has
no server, no account and no analytics. It uses the Accessibility API **only to
find where the battery icon is on the status bar**, and never reads what is on
your screen. Purchases are handled entirely by Google Play.

### 1. Information we collect

**None.** We (the developer) receive no personal information, usage data,
telemetry, crash reports or analytics of any kind.

### 2. Information stored on your device

Battery Charm stores the following in its own private app storage:

| Stored | Why |
|---|---|
| Your decoration settings — chosen theme, backdrop, size, chain length, swing feel, battery digit style | To draw the decoration you chose. |
| Images you import as a backdrop, and the image you choose for the lock screen (alternative mode) | Copied into app storage so the decoration keeps working even if the original is moved. Only images you pick yourself through the system picker are read. |
| The measured position of the battery icon for this device | To place the decoration precisely. Kept on this device only. |
| Points, themes unlocked with points, and the date of the last daily bonus | For the free points system. |
| Whether you own Pro (a copy of your Google Play purchase status) | So Pro keeps working offline. Google Play remains the source of truth. |

You can delete all of it by clearing the app's data or uninstalling the app.

**Android backup.** Your decoration settings and your points / unlocked themes
are included in Android's standard backup to **your own Google account**, so they
come back when you reinstall or move to a new phone. Images, the battery icon
position and the Pro copy are **not** included. This backup is operated by
Google under your Google account; we cannot access it. You can turn it off in
your phone's backup settings.

### 3. Network usage

Battery Charm's own code makes **no network connections**. The app does declare
the `INTERNET` permission, because the **Google Play Billing Library** (used for
the Pro purchase) requires it to talk to Google Play. No data from the app is
sent to us or to any other party.

### 4. Permissions and why they are required

| Permission | Why |
|---|---|
| Accessibility service (`BIND_ACCESSIBILITY_SERVICE`) | Used **only to read the on-screen position of the status bar's battery icon and system icons**, so the decoration can be drawn exactly around them. It does **not** read screen content, text you type, notifications or any other app's data, does not perform actions on your behalf, and stores or sends nothing it reads. You turn it on yourself in system settings after an in-app explanation. It is not presented as an accessibility tool for people with disabilities. |
| Display over other apps (`SYSTEM_ALERT_WINDOW`) | Alternative mode only (when you choose not to use the accessibility service): to draw the decoration on top of the screen. |
| Foreground service (`FOREGROUND_SERVICE`, `FOREGROUND_SERVICE_SPECIAL_USE`) | Alternative mode only: to keep the decoration displayed. Shows an ongoing notification while it runs. |
| Notifications (`POST_NOTIFICATIONS`) | To show that ongoing notification, with a button to turn the decoration off. |
| Set wallpaper (`SET_WALLPAPER`) | Alternative mode only: to set a lock screen wallpaper that has the decoration drawn onto the image you chose. The app does not read your current wallpaper. |
| Run at startup (`RECEIVE_BOOT_COMPLETED`) | To show the decoration again after the phone restarts. |
| Google Play billing (`com.android.vending.BILLING`), `INTERNET`, `ACCESS_NETWORK_STATE` | Added by the Google Play Billing Library for the Pro purchase. |

The battery level and charging state come from Android's standard battery
broadcast, which needs no permission.

### 5. Third-party services and SDKs

- **Google Play Billing Library** — processes the one-time Pro purchase. Payment
  details are handled by Google Play and are never visible to the app or to us.
  The app only learns whether Pro is owned. See
  [Google's Privacy Policy](https://policies.google.com/privacy).
- AndroidX / Jetpack libraries from Google (Compose, DataStore) used for app
  structure. They do not transmit user data.

There are **no** ads, analytics or crash reporting libraries.

### 6. Children's privacy

Battery Charm is not directed at children under 13. The app knowingly collects
no data from anyone, including children.

### 7. Changes to this policy

This policy may be updated as the app evolves (for example, if rewarded ads are
added in the future, this page will be updated before that version is
released). Updates are reflected by changing the "Last updated" date at the top
of this page.

### 8. Contact

[contact@13each.com](mailto:contact@13each.com)

---

<a id="japanese"></a>

## 日本語

### 要約

バッテリーチャームは**個人データの収集・販売・共有を一切行いません**。サーバー、
アカウント、解析はありません。アクセシビリティ API は**ステータスバーにある電池
アイコンの位置を知るためだけ**に使い、画面の内容は読みません。購入の処理はすべて
Google Play が行います。

### 1. 収集する情報

**ありません。** 開発者が個人情報、利用状況、テレメトリ、クラッシュレポート、
解析データを受け取ることはありません。

### 2. 端末内に保存される情報

アプリ専用の保存領域に、次のものを保存します。

| 保存するもの | 目的 |
|---|---|
| デコの設定 — 選んだテーマ、背景、大きさ、チェーンの長さ、揺れ方、電池の数字の見た目 | 選んだデコを描くためです。 |
| 背景として読み込んだ画像と、ロック画面用に選んだ画像 (代替モード) | 元の画像を移動してもデコが表示されるよう、アプリ内にコピーします。読むのは、システムの選択画面でご自身が選んだ画像だけです。 |
| この端末で測った電池アイコンの位置 | デコを正確な位置に置くためです。この端末の中だけに置きます。 |
| ポイント、ポイントで開けたテーマ、最後にログインボーナスを受け取った日 | 無料のポイントのためです。 |
| Pro を持っているか (Google Play の購入状態の写し) | オフラインでも Pro が使えるようにするためです。正しい情報は Google Play 側にあります。 |

アプリのデータを消去するか、アンインストールすると、すべて消えます。

**Android のバックアップについて。** デコの設定とポイント・開けたテーマは、
Android 標準のバックアップで**ご自身の Google アカウント**に保存され、入れ直しや
機種変更のときに戻ります。画像、電池アイコンの位置、Pro の写しは**含みません**。
このバックアップは Google がご自身のアカウントで運用するもので、開発者は見ることが
できません。端末のバックアップ設定でオフにできます。

### 3. ネットワークの利用

アプリ自体のコードは**ネットワークに接続しません**。ただし、Pro の購入に使う
**Google Play 請求サービスのライブラリ**が Google Play と通信するために必要と
するため、`INTERNET` 権限を宣言しています。アプリのデータが開発者やほかの誰かに
送られることはありません。

### 4. 権限とその理由

| 権限 | 理由 |
|---|---|
| ユーザー補助サービス (`BIND_ACCESSIBILITY_SERVICE`) | **ステータスバーにある電池アイコンとシステムアイコンの、画面上の位置を読むためだけ**に使います。その周りにデコをぴったり描くためです。画面の内容、入力した文字、通知、ほかのアプリのデータは**読みません**。代わりに操作することもなく、読んだものを保存・送信することもありません。アプリ内の説明のあと、ご自身がシステム設定でオンにします。障がいのある方向けの支援ツールとしては提供していません。 |
| ほかのアプリの上に重ねて表示 (`SYSTEM_ALERT_WINDOW`) | 代替モード (ユーザー補助を使わない場合) のみ。デコを画面の上に描くためです。 |
| フォアグラウンドサービス (`FOREGROUND_SERVICE`、`FOREGROUND_SERVICE_SPECIAL_USE`) | 代替モードのみ。デコを表示し続けるためです。動いている間は通知を表示します。 |
| 通知 (`POST_NOTIFICATIONS`) | その通知と、デコをオフにするボタンを表示するためです。 |
| 壁紙の設定 (`SET_WALLPAPER`) | 代替モードのみ。ご自身が選んだ画像にデコを描いて、ロック画面の壁紙に設定するためです。今の壁紙は読みません。 |
| 起動時の実行 (`RECEIVE_BOOT_COMPLETED`) | 端末を再起動したあと、デコをもう一度表示するためです。 |
| Google Play の購入 (`com.android.vending.BILLING`)、`INTERNET`、`ACCESS_NETWORK_STATE` | Pro の購入のため、Google Play 請求サービスのライブラリが追加します。 |

電池の残量と充電中かどうかは、権限のいらない Android 標準のお知らせから得ています。

### 5. 第三者のサービス・SDK

- **Google Play 請求サービスのライブラリ** — Pro の買い切りの購入を処理します。
  支払いの情報は Google Play が扱い、アプリや開発者が見ることはありません。アプリが
  知るのは Pro を持っているかどうかだけです。
  [Google のプライバシーポリシー](https://policies.google.com/privacy) をご覧ください。
- アプリの構造に使う Google の AndroidX / Jetpack ライブラリ (Compose、DataStore)。
  ユーザーデータは送信しません。

広告、解析、クラッシュレポートのライブラリは**含みません**。

### 6. 子どものプライバシー

13歳未満の子どもを対象としていません。子どもを含め、誰からもデータを収集しません。

### 7. 本方針の変更

アプリの変更に合わせて本方針を更新する場合があります (たとえば今後、広告を見て
ポイントをもらう機能を加える場合は、そのバージョンを出す前にこのページを更新します)。
更新はページ上部の「Last updated」の日付で示します。

### 8. お問い合わせ

[contact@13each.com](mailto:contact@13each.com)

---

<a id="korean"></a>

## 한국어

### 요약

Battery Charm은 **어떤 개인 데이터도 수집·판매·공유하지 않습니다.** 서버, 계정,
분석 도구가 없습니다. 접근성 API는 **상태바에 있는 배터리 아이콘의 위치를 찾는
데만** 쓰고, 화면 내용은 읽지 않습니다. 결제는 모두 Google Play가 처리합니다.

### 1. 수집하는 정보

**없습니다.** 개발자는 개인정보, 사용 기록, 텔레메트리, 크래시 리포트, 분석
데이터 중 어떤 것도 받지 않습니다.

### 2. 기기에 저장되는 정보

앱 전용 저장 영역에 아래 항목을 저장합니다.

| 저장 항목 | 목적 |
|---|---|
| 꾸미기 설정 — 고른 테마, 배경, 크기, 체인 길이, 흔들림, 배터리 숫자 모양 | 고른 꾸미기를 그리기 위해서입니다. |
| 배경으로 가져온 이미지와 잠금화면용으로 고른 이미지 (대체 모드) | 원본을 옮겨도 꾸미기가 계속 보이도록 앱 안에 복사합니다. 시스템 선택 화면에서 직접 고른 이미지만 읽습니다. |
| 이 기기에서 측정한 배터리 아이콘 위치 | 꾸미기를 정확한 위치에 놓기 위해서입니다. 이 기기 안에만 둡니다. |
| 포인트, 포인트로 연 테마, 마지막으로 출석 보너스를 받은 날짜 | 무료 포인트 기능을 위해서입니다. |
| Pro 보유 여부 (Google Play 구매 상태의 사본) | 오프라인에서도 Pro를 쓸 수 있도록 하기 위해서입니다. 정확한 정보는 Google Play에 있습니다. |

앱 데이터를 삭제하거나 앱을 제거하면 모두 지워집니다.

**Android 백업.** 꾸미기 설정과 포인트·연 테마는 Android 기본 백업으로
**사용자 본인의 Google 계정**에 저장되어, 앱을 다시 설치하거나 기기를 바꿀 때
돌아옵니다. 이미지, 배터리 아이콘 위치, Pro 사본은 **포함하지 않습니다.** 이 백업은
Google이 사용자 계정으로 운영하며, 개발자는 볼 수 없습니다. 기기의 백업 설정에서 끌
수 있습니다.

### 3. 네트워크 사용

앱 자체 코드는 **네트워크에 연결하지 않습니다.** 다만 Pro 구매에 쓰는
**Google Play 결제 라이브러리**가 Google Play와 통신하는 데 필요해서 `INTERNET`
권한을 선언합니다. 앱의 데이터가 개발자나 다른 누구에게 전송되지 않습니다.

### 4. 권한과 필요한 이유

| 권한 | 이유 |
|---|---|
| 접근성 서비스 (`BIND_ACCESSIBILITY_SERVICE`) | **상태바에 있는 배터리 아이콘과 시스템 아이콘의 화면 위치를 읽는 데만** 씁니다. 그 주위에 꾸미기를 딱 맞게 그리기 위해서입니다. 화면 내용, 입력한 글자, 알림, 다른 앱의 데이터는 **읽지 않습니다.** 앱을 대신 조작하지 않으며, 읽은 것을 저장하거나 전송하지 않습니다. 앱 안의 안내를 본 뒤 사용자가 직접 시스템 설정에서 켭니다. 장애인 지원 도구로 제공하지 않습니다. |
| 다른 앱 위에 표시 (`SYSTEM_ALERT_WINDOW`) | 대체 모드(접근성을 쓰지 않을 때)에서만. 꾸미기를 화면 위에 그리기 위해서입니다. |
| 포그라운드 서비스 (`FOREGROUND_SERVICE`, `FOREGROUND_SERVICE_SPECIAL_USE`) | 대체 모드에서만. 꾸미기를 계속 표시하기 위해서입니다. 실행 중에는 알림을 표시합니다. |
| 알림 (`POST_NOTIFICATIONS`) | 그 알림과 꾸미기를 끄는 버튼을 보여주기 위해서입니다. |
| 배경화면 설정 (`SET_WALLPAPER`) | 대체 모드에서만. 사용자가 고른 이미지에 꾸미기를 그려 잠금화면 배경으로 설정하기 위해서입니다. 현재 배경화면은 읽지 않습니다. |
| 부팅 시 실행 (`RECEIVE_BOOT_COMPLETED`) | 기기를 다시 켠 뒤 꾸미기를 다시 표시하기 위해서입니다. |
| Google Play 결제 (`com.android.vending.BILLING`), `INTERNET`, `ACCESS_NETWORK_STATE` | Pro 구매를 위해 Google Play 결제 라이브러리가 추가합니다. |

배터리 잔량과 충전 여부는 권한이 필요 없는 Android 기본 배터리 알림에서 얻습니다.

### 5. 제3자 서비스 및 SDK

- **Google Play 결제 라이브러리** — Pro 일회성 구매를 처리합니다. 결제 정보는
  Google Play가 다루며, 앱이나 개발자는 볼 수 없습니다. 앱이 아는 것은 Pro 보유
  여부뿐입니다. [Google 개인정보처리방침](https://policies.google.com/privacy)을
  참고하세요.
- 앱 구조에 쓰는 Google의 AndroidX / Jetpack 라이브러리(Compose, DataStore).
  사용자 데이터를 전송하지 않습니다.

광고, 분석, 크래시 리포트 라이브러리는 **포함하지 않습니다.**

### 6. 아동의 개인정보

13세 미만 아동을 대상으로 하지 않습니다. 아동을 포함해 누구에게서도 데이터를
수집하지 않습니다.

### 7. 본 방침의 변경

앱이 바뀌면 이 방침을 갱신할 수 있습니다 (예: 앞으로 광고를 보고 포인트를 받는
기능을 넣는다면, 그 버전을 내기 전에 이 페이지를 먼저 갱신합니다). 갱신은 페이지
상단의 "Last updated" 날짜로 표시합니다.

### 8. 문의

[contact@13each.com](mailto:contact@13each.com)
