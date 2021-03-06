用語集
######

.. glossary::

    ルーティング配列
        :php:meth:`Router::url()` に渡される属性の配列。
        典型的には以下のようになります。 ::

            ['controller' => 'Posts', 'action' => 'view', 5]

    HTML属性
        HTMLの属性を構成するキー => 値の配列。例::

            // これを与えると
            ['class' => 'my-class', 'target' => '_blank']

            // これが生成される
            class="my-class" _target="blank"

        オプションが最小化できるか、名前そのもが値として許可される場合は、
        ``true`` が利用できます。 ::

            // これを与えると
            ['checked' => true]

            // これが生成される
            checked="checked"

    プラグイン記法
        プラグイン記法はドットで区切られたクラス名で、クラスがプラグインの一部であることを
        指定しています。 ::

            // プラグインは "DebugKit", クラス名は "Toolbar".
            'DebugKit.Toolbar'

            // プラグインは "AcmeCorp/Tools", クラス名は "Toolbar".
            'AcmeCorp/Tools.Toolbar'

    ドット記法
        ドット記法は、 ``.`` を用いてネストされたレベルを区切ることによって配列のパスを定義します。
        例::

            Cache.default.engine

        は以下の値を指し示します。 ::

            [
                'Cache' => [
                    'default' => [
                        'engine' => 'File'
                    ]
                ]
            ]

    CSRF
        クロスサイトリクエストフォージェリ(*Cross Site Request Forgery*)。
        再生攻撃、二重投稿、他ドメインからの偽造リクエストを防止します。

    CDN
        Content Delivery Network の略。世界中のデータセンターにあなたのコンテンツを
        配信するために利用するサードパーティベンダーです。地理的に分散したユーザーの近くの
        静的なアセットを送信するのに便利です。

    routes.php
        ``config`` ディレクトリ中のファイルで、ルーティングの設定が入っています。
        このファイルは全てのリクエストが処理される前に読み込まれます。リクエストが正しい
        コントローラ+アクションにルーティングされるように、アプリケーションが必要とする
        全てのルートに接続する必要があります。

    DRY
        同じことを繰り返さない (Don’t repeat yourself)。これはあらゆる情報の繰り返しを
        少なくするためのソフトウェア開発の原則です。CakePHP では同じコードは１カ所に書いて
        再利用するという形で DRY 原則に従っています。

    PaaS
        Platform as a Service の略。クラウドベースのホスティング、データベース、
        キャッシュリソースを提供します。有名なプロバイダーは、Heroku、EngineYard、
        PagodaBox などです。

    DSN
        データソース名。URI のような書式の接続文字列フォーマット。CakePHP は、キャッシュ、
        データベース、ログ、Eメール接続のための DSN に対応します。


.. meta::
    :title lang=ja: 用語集
    :keywords lang=ja: HTML属性,配列クラス,配列コントローラ,用語集,target blank,ドット記法,ルーティング設定,forgery,replay,ルーター,シンタックス,config,submissions
