/**
 * Loggix_Plugin - Optimize DB
 *
 * @copyright Copyright (C) UP!
 * @author    hijiri
 * @link      http://tkns.homelinux.net/
 * @license   http://www.opensource.org/licenses/bsd-license.php  New BSD License
 * @since     2010.06.13
 * @version   10.7.14
 */

●データベースのバックアップと最適化を行うプラグイン

■概略
このソフトウェアは、Loggixのデータベースファイルのバックアップと最適化を自動で行うプラグインです。

■詳細
ガーベジコレクションとVACUUMを予め指定した日数(標準では10日)毎に行います。また、その際に自動的にバックアップを作成します。

■インストール/アンインストール方法
インストール
    1./data/loggix.sqlite3.dbを念の為FTP等でローカルへダウンロードする等してバックアップしておきます。
    2./plugins/へoptimizeDB.phpをアップロードします。必要であれば、プラグインを実行する日数を修正します。

アンインストール
    1./plugins/からoptimizeDB.phpを削除します。

■使用方法
インストール後Loggixへブラウザでアクセスします。以後は予め指定した日数毎にバックアップと最適化が行われます。

■その他
対応するデータベースファイルはSQLite3のみになります。また、バックアップファイルは常に/data/loggix.sqlite3.db.BAKとなり世代管理は出来ません。

■サポート
作者多忙の為サポート出来ません。意見/感想はContactからご連絡ください。

■更新履歴
2010-07-14:公開