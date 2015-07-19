## トランザクションの使用

Aliceのトランザクションは、ブロックの一部としてブロックチェーンに組み込まれたことで、全てのビットコイン・アプリケーションからそのトランザクションを参照できるようになりました。それぞれのクライアントはトランザクションの有効性を独自に検証することができます。フル・インデックス・クライアントは資金の出自を、最初にその資金が採掘により生み出されたときからBobのアドレスに渡るまでのすべてのトランザクションを追うことができます。軽量クライアントであれば、簡略支払認証（SPV: Simplified Payment Verification）として、資金の元となったトランザクションが、ブロックチェーン内のブロックに組み込まれており、そのブロックより後にいくつかのブロックが存在することを確認し、ネットワークがそのトランザクションを正当と判断してくれることを担保します (詳細は<<spv_nodes>>節を参照)。

Bobは、Aliceとのトランザクションのアウトプットを別のトランザクションのインプットとして新しいオーナーを割り当てることで、受け取った資金を支払いに使うことができます。例えばAliceのコーヒーカップの支払いを請負業者や納入業者への支払いに利用することが可能です。また、たくさんの細かい支払いを一つのトランザクションに集約することもよく行われます。たとえばBobの本日の売り上げを決済用の口座として使っているアドレスに集約するような使われ方をするかもしれません。この集約については、[先ほどの図](00_images/msbt_0206.png)を参照してください。

BobがAliceや他の人から受け取った資金を利用することで、トランザクションの連鎖が広がり、結果、ブロックチェーンにも書き込まれていきます。ここではBobがバンガロールのWebデザイナーであるGopeshに支払うことを考えましょう。トランザクションの連鎖は 下図のようになります。

!["JoeからGopeshへの一連のトランザクション"](00_images/msbt_0210.png "JoeからGopeshへの一連のトランザクション")