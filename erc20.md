※毎回細かいこと忘れるので，フロー書いてく（随時加筆）．

## 1. 初期
- mkdir & cd
- ```
  truffle init
  ```
- `truffle.js`において，**Ganache**によるローカルネットワークの設定を追記する．

    ```
    networks: {
        development: {
            host: "127.0.0.1", // 仮
            port: "7545", // 仮
            network_id: "*" // match any network id
        }
    }
    ```
- Ganache起動．上記ネットワーク設定を調整
- Metamaskのネットワーク切り替えも忘れるな

## 2. コントラクト
- tokenコントラクトを作成
- tokenコントラクトのマイグレーションファイルを作成
- ```
  truffle migrate
  ```
- テストコードを作成
- tokenのクラウドセール(ICO等)のコントラクトを作成
- ```
  truffle migrate
  ```

## 3. テストネットワーク(Rinkeby)
- gethでアカウントを作ったり，同期を開始する
- faucetサイトでethをもらう
- ```
  truffle migrate --reset --compile-all --network rinkeby
  ```

## 4. クライアントとの接続
- よしな of よしな
