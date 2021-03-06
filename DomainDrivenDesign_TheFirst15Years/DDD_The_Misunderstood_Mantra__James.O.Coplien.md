# DDD The Misunderstood Mantra (DDD誤解のマントラ)

- 著者
    - James.O.Coplien

---

- ドメインレベルの思考が重要
    - プログラマーはオブジェクトレベルの近視的になりがち
    - パターンはこの考えへの見通しがあったが、まだまだ少なかった
    - DDDはユビキタス言語としてドメインレベルに対する意識を高める効果があった
        - ユビキタス言語の集まりは優れたデザインを生み出すきっかけとなる










---
# Google訳


エリック、あなたのマグナムオーパスの15周年記念であなたに演説するために招待された人々の会社に私が自分自身を見つけることができてうれしい、そして光栄です。  
私も、このプロセスに15年間携わってきました。そして、私たちの両方のアイデアが成長していくのを見てきました。  
DDD Europeであなたに会えたことは私にとってのハイライトであり、あなたから直接学ぶことができる初めての機会でした。  
私はまだそのプロセスを続けることを切望しています、そして、私たちがすぐにまた対面で会うことを願っています。  
その間、これはそれらの議論のためのポンプを準備するあなたへの手紙のようです。
私はこれらのアイデアを、私たちが次に学ぶことに最大の敬意と大きな期待を持って提供します。
これは私達の共有された願望を振り返り、そして私達が私達の心の中で運んでいるアイデアの交換のために火を燃やすために私達の過去の議論のいくつかのトピックを再検討する絶好の機会です。
私たちが論じたように、思考の多くは、表面的な理解（そして誤解）を超えてあなたが伝えようとしていたアイデアの深さに人々を引き込む方法でメッセージを提示する方法に関連しています。この小さなプロジェクトを私が経験豊かで思いやりのある同僚としてだけでなく、友人としてもカウントする人にとっての驚きとして進むことは、楽しくて強力です。  
そして、この会話を直接続けていくために、いつの日か池の向こうにあなたが一緒にいることを願っています。

---

### Foreword

2016年に私がDDDヨーロッパで話をしたとき、Eric Evansと私は、ドメイン駆動設計（DDD）を本当に理解している人はほとんどいないと公言しました。  
それは10代のセックスについての古い冗談にふさわしい：誰もがそれについて話していてそれをしたいと思っています、本当にそれをしている人はほとんどいません、そしてそれをひどくしている人はいません。  
たとえ私が自分自身について頭を悩ませていたとしても、そしてEricと話をしている時でさえ、彼はAddison-Wesleyがその初期の日にそれをレビューするよう私に頼んだ時とは違って本を書くでしょう。  
これらの考察は、これらの考えの歴史の15年に関する一つの見方を示しています。  
15年経っても作品の歴史的な場所を評価するには時期尚早です。それにはさらに10年かかる、と私は思います。  
しかし、おそらく私の現在の考えは、Ericが自分の達成したことに誇りを持っていることと、同僚と一緒に彼に挑戦して既存の基盤に新しい考えや洞察を加えることができるでしょう。  
私がここで言っていることの多くは、Ericがすでに彼の頭の中にいることに疑いを持っていません。  
もしそうなら、そんなに良い。


### First Impressions

2002年に、Ericの本について私が最初に驚いたことの1つは、彼がオブジェクト指向プログラミングのもう1つの原理主義者ではなかったということです。  
特にデザインにおけるドメインビューは、当時の文献では見つけるのが困難でした。  
業界は、これまでと同様、その欠点を直すのに苦労していました。  
私自身の仕事は、オブジェクトレベル近視から私たちを解放することにおいて、ドメインレベルの思考が貴重であることを発見しました、一方、業界の大部分はファッショナブルになって以来オブジェクトコミュニティでしばしば見いだされた。  
パターンはこの見通しを和らげるためにいくつかの侵入をしましたが、このレベルで考え方を共有した他のアイデアはほとんどありません。  
Ericの仕事はいくつかの未開封の宝箱を開くことでした。  
私の考えでは、Ericが行った最も重要な貢献は、彼がユビキタス言語と呼んでいるものに対する意識を高めることです。
それは普遍的ではなく、確かに言語ではありませんが、そのような言葉の集まりは、優れたデザインが生み出される弁証法の根拠となります。  
それについては後で詳しく説明します。

---

しかし、この本について2つのことが私を少し悩ませました。   
1つは、大規模なドメイン分析に関する文献をまったく呼び出さなかったことです。
コンピュータサイエンス分野では、ビジネスのアプリケーション分野とソリューション分野の両方で、焦点または知識の分野を明確にします。  
プログラムの進化の下で回復力のあるドメインを見つけるには十分な分析が必要であり、この本はそれには興味がありませんでした - この分野はよく知られていますが。  
4年前からのマルチパラダイムデザインに関するこの分野での私自身の仕事のおかげで、私はこの観点に私の自我を少し投資したのかもしれません。  
その文献の多くをソフトウェアエンジニアリングのコミュニティに結び付けている人はいませんでした。  
そ   の当時は、ソフトウェアエンジニアリングとオブジェクトコミュニティの間にはほとんど関連性がないと言っても過言ではありません。  
それでも、本のタイトルに最も重要な単語ドメインを使用している人が、ドメインエンジニアリングとドメイン分析という豊富な出版物の遺産に敬意を表していないことに私は困惑しました。  
 （グーグルは、ドメインエンジニアリングに1億8,300万ヒット、ドメイン駆動デザインに1億1,600万ヒットしている。）

---

もっと広く言えば、この本は、当時5歳くらいだったXPで見つかるのと同じ感情の多くを呼び起こしているように見えた。  
そのため、この本はパラドックスであり、どちらも当時の修辞学から離れていましたが、同時にその時代の分析の過少評価を受け入れていました。  
XPは意識的に従来の知恵と180°位相がずれていました。 
優れた分析を行うことは、当時の常識の一部でした。つまり、デザインに飛び込む前に、エンドユーザーにビジネスの視点を正しく認識させることです。  
代わりに、XPはオンサイトの顧客を、ユーザーのニーズと開発者の空想の間にギャップが生じる可能性に対する保険ポリシーとして使用します。  
DDDは、当時のオタク精神主義者に身を置いていました。  
意識的に分析から離れている間それはデザインを受け入れるでしょう。

---

その時代の分析文化がひどく再起動を必要としていたことは否定できません。  
この頃になっても「ウォーターフォール」という用語は4文字の単語になり、ほとんどの人にはわからないようになっていましたが、広範な慣習ではまだ「滝の開発」に関連した広範な慣行が証明されています。  
世界はウォーターフォールから走り始めました。それは人々が彼らが走るべきである原因をまだ立証していなかった不快な時代でした。  
フレームワーク、パターン、そしてプログラミング言語の機能は、当時の共有スペースを埋めるために拡張されました。  
次の方法、特にXPを超える規模の方法を待っていた人たちは確かにいました - 前の時代からの管理領域に直面して、単一チームの開発を超えて何かをサポートできるという主張をしませんでした。まだスケーリングを信じていました。  
 （そして、残念なことに、これは約15年後にメソッドの世界で生まれ変わった視点です。）

---

新しい熱狂者は風呂水でことわざの赤ちゃんを捨てた。  
後の研究では、実際には、皇帝の新しい極値は、私たちがマーティン、ビドル、ノーブル、アブラハムソン、シニアアルト、その他の著名な論文に見られるように、以前の政権のものと同じくらい悪いことが指摘されるでしょう。  
Martinは、オンサイトの顧客が「持続不可能」であることを発見しました（XP顧客の役割）。  
AbrahamssonやSiniaaltoを含む多くの人がTDDがその約束を守らなかったことを知っていました。  
しかし2002年になって、ほとんど1年前のアジャイル宣言の影で、あなたはアジャイルではなかったと言うのはほとんど共産主義者でした、そしてあなたは確かにあなたの時代の頭を語っている主流の方法の怒りを招くでしょう「アジャイル」という概念には、オンサイト顧客およびTDDが含まれていないか、「分析」という用語がささやいている場合は含まれていません。  


ドメイン駆動設計はこの観点と適切に一致していましたが、フレーミングは明らかにXPに似ていませんでした。  
本は、それ自身の分野、人工物、そしてとりわけ十分な、それ自身の語彙を持つ成熟した、よく考え抜かれたそして実践されたアプローチのすべての罠を持っていました。  
これらすべては本に権威の十分にふさわしい空気を与えました。  
私は、アジャイルな人々が分析分野で捨てていたことを、DDDがデザインに押し戻そうとしたと思います。  
複雑なソフトウェアの設計、実装、およびテストを分離することは愚かなことであり、それは滝から外れた最初の罠の1つであることを長年にわたって学んできました。  
しかし、分析と生産の二分法は残っていました。例えば、スクラムでは、この二分法はプロダクトオーナーの役割に属しています。  
ここで、DDDの本では、分析の懸念を設計表に持ち込もうとしたように見えました。  
そしてもちろんこれは理論的には、あるいは経験豊富で統制のとれた開発者の手には役立ちます。  
実践は、DDDの本が行うよりも大きな節度を求めて分析を祝うに値するが、その時代の一般的な実践で見られるものよりもはるかに少ない。
そのように、DDDの本は荒れた、進行中の対話の産物でした。  
エリックは彼の経験に基づいて、彼がした場所に賭け金を置くことにしました。  
彼の経験は、洞察力やビジネス知識、あるいはその両方を熱心に持っていた開発者や指導者たちによって、際立った特徴を持っていなかったと私は考えることができます。  
 その場合、何でもうまくいき、DDDの世界モデルは、その作品を構造化するためのものと同じくらい良い方法でした。
 
 --- 
 
 私は、Ericがここで何かをしているのではなく、流れを続けていることを強調していると思う。  
 20世紀後半に疑似アジャイルの多くの練習に懐疑的な人として、他の日和見主義者たちと一緒にEricをひとまとめにするのは簡単なので、私にとって言うことは重要です。  
 彼の考えと彼らの考えとの間の重複に基づいて。  
 彼が提案していたのは、その構造の程度においてアジャイルの人々に急進的であり、そして分析を避けて伝統主義者に急進的だった。  
 彼がその本性によって当時の流行に直面して飛んだ分野、構造および語彙を含んでいたことは、エリックが本を売るかまたは名声を求めるより深い何かによって動機を与えられたと言います。  
 2016年まで個人的に彼と知り合うことはできませんでした。私にはすぐに明らかになりました。エリックを知っている人には明らかだと思います。  
 彼は何かを深く正しいことを発見したという気持ち、そしてあまり多くの人が自分で発見していないことを動機付けています。  
 私は彼の論文のいくつかの点で彼に反対するかもしれないが、
 どういうわけか問題ではありません。
 私たちは同じ探究プロセスと同じ動機を共有しています。  
 私にはそれで充分です。
 そしてそれはここで分析と対応点の基礎を築きます。   
 しかし、私はdigressをします。

---
私はDDDの本を複雑なシステム開発の領域の観点からよく考えてきました。  
私のキャリアのおかげで、過去35年間、そのドメインをそれ自体で現象または物として勉強するようになりました。  
この間に、複雑なシステム開発の理論を開発できるようになりました。その理論は、Christopher Alexander、Peter Senge、Russell Ackhoffなど、私たちの分野以外の人々に大きく依存しています。  
スクラムは、その理論を明示的に利用する最初の現代的な方法の1つです。  
しかし、DDDの本は、開発文化を超越し、おそらく個人的な洞察と経験の偶然の違いを補うであろう理論を利用することに大失敗しました。  
そして、そのようなことは自分自身の経験から引き出されたものであるように、それはある時には機能し、ある時には機能しません。  
XPとは異なりますが、それは適用性の同じ課題に直面しました。  

---
ただし、EricやDDDとは関係がありませんが、それが私たちの学問分野全体を覆い隠しているため、気にする必要があるはずです。  
一例として、広く使用されていて1990年代初頭までに明確に定義されているドメイン固有言語（DSL、アプリケーション指向言語またはAOLとも呼ばれる）を考えてみましょう。  
Martin Fowlerは、ドメイン固有の言語という古くからの概念を取り入れ、既存の汎用言語のプログラムに埋め込まれている規則の意味でそれを使い始めました。  
うまく構造化された言語で適切に選択された識別子によってコードが理解しやすくなるという点で、この背後には洞察の核があります。  
それでも、言語は、単語間の関係をどのように構成するかに関するものであるため、識別子以上のものです。  
最近のほとんどのプログラミング言語でも、構文をFORTRAN（宣言、代入）までさかのぼります。一般的な言語の基本的な型とセマンティクスは、まだ代数演算子です。  
コンピューティングはもともと数字で遊ぶことでしたが、私たちは長い道のりを歩んできました、そして本当のDSLは単なる語彙を超えて本当の言語へと行きます。  

---

言語は構文だけでなく意味論も持っています - そして言語の最も強力な意味論のいくつかはその慣用句にあります。  
そして、DSLと呼ばれるようになったことに最も興味を持っているのは、言語ではなく語彙のレベルであり、ドメインではなく当面の関心事です。  
そのため、現代のDSLは、システム構造全体のラクダを無視しながら、ローカル表現の癖を絞り込むことになりました。  
言語はフォームについての考え方をエンコードしており、ドメイン指向の考え方の分野の多くはそれらが組織するフォームについてです。  
これらの形式を適切な語彙で表現することは、ほとんど脚注です。    
AOLとDSLの1980年代初期の伝統は、これらの基本的な形式を捉えるためにゼロから言語を構築しましたが、皇帝の新しいDSLは同じ辞書（文法、構文、および基本セマンティクス）を使用します。  
それはユビキタス言語が言語かユビキタスのどちらかであるというふりをするのと平行しています。  

---

しかし、あなたが2000年以降の新世代のオタクと話をした場合、彼らがDSLを知っていれば、彼らはFowlerのDSLの概念を振り返るでしょう。  
おそらくその理由は、優れたDSLを実行するには手に負えない分析投資が必要であるということです。  
分析が時代遅れであるため、概念を抜粋して何か他のものを作成することが必要になりました。  
あるいは、DSLは、安定していないドメインでは非常に悪い結果を招く傾向があります。  
数学の領域はかなり安定しているので、Excel®のようなDSLはかなりうまくいきます。  
パーサー理論は健全で安定しているので、yaccとbisonはそれほど変わらない。  
 （頻繁なantlrの変更は面倒であり、構文サッカリンに達し、現状に追いついているようです。）  
それでも、皇帝の新しいDSLはDDDアプローチの中心になることを目指しています。それらは分析ではなくデザインです。  
彼らはユビキタス言語の概念を受け入れるためにやや拡張可能な言語に基づいています。  
また、Excel®やyaccのような堅牢な言語とは異なり、どのコーダーでも都合の良いときに言語を進化させることができます。  

---


Ericは私達に私達の設計決定のためのオラクルとして役立つべきであるドメインと呼ばれるNorth Starを見せようとしたと思います。  
ドメインに相談せずにさりげなくDSLを変更するべきではありません。  
Ericのドメインは、何らかの理由で、法律よりも慣習が多いと感じています。  
また、従来のドメイン分析コミュニティ（Neighbors、Lai、Weiss、Parnasなど）は、その根拠に近いと主張しています。  
ソフトウェアが提供していた企業。しかし、Ericのドメインは、概念を表現するためにどれだけタイプする必要があるかという、開発者の日常的な用語の重要性に対する感覚よりも確かに自明です。  
そして新しい時代のDSLはステロイド上のマクロにすぎないようです。  
そして彼のドメインの概念がそのマークを見逃した場合、ユビキタスな言語の彼の概念はブルズアイに当たる - たとえそれが語彙についてだけであっても。  
言葉は物事を意味し、私はエリックのように理解している人はほとんどいないと思います。  

---


## Reflection(自省 / 回想)

### Guild not the lily

- guild the lily  
    - シェイクスピアのジョン王から
    - 既に完璧なものに余計な手を加える(ユリを黄金に変える）


私は、DDDのアイデアの理論的根拠を見つけることができないという私の欲求不満について語った。  
これは根本的な命題を思い起こさせます。  
実際には、建物を構造化するための正式な根拠がある以上に、プログラム構造に理論的根拠はありません。  
確かに、建物は立っていなければならず、プログラムはコンパイルしてリンクしなければなりませんが、それらは科学の問題よりもエンジニアリングの問題です。  
経験的観点から見ても、グッドデザインの理論や原理を引き出すことは困難です。  
そしてこの本は、懸念の分離やAPIへの注意など、私たちが同意することを強調しています。  


---

たとえば、ドメインアナリストの実績はさまざまです。  
その意味論が計算の公理に基づいているyaccやExcelのような成功があります。  
SQLについても同様のことが言えます。  
ソフトウェア開発の最も複雑な分野では、そのような正式な根拠を享受していません。  
そのため、分析の杭打ちを地面に置くことは悪魔的に困難になります。  
私はこれらの努力の多くを見てきました、ドメイン分析、カレイ、創始者に根ざし、そして最終的に失敗します。  
彼らは1970年代の滝の、重くて過度に前に積まれた努力を思い出す傾向があります。  


---

これは、ソフトウェア工学の伝統に反する、クラフトプログラミングという別の実行可能な見方があるかどうかについて疑問を投げかけます。  
私は、多くのソフトウェアエンジニアリングの問題を軽視していますが、おそらくEricに加わって同僚にさらに軽蔑するように勧めてください。  
Ericの本は、一見すると、ソフトウェア工学の分野の話題を扱っているという点で不思議な本です。  
ソフトウェア工学の文献とEricの本の両方とも、彼らの中核的なアイデアについて信頼できる根拠を持っていませんが、それはアイデアが間違っているという意味ではありません。  
どちらの場合でも、普遍性が見つかることはまずありません。

---

ある意味で、オブジェクト指向、トップダウンデザイン、またはウォーターフォールの原理主義者たちを批判するのと同じように、私は罠に陥ったかもしれません。  
それらのどれかが「機能する」かどうかという貴重な小さな証拠があります。  
ウォーターフォールは私たちを月に乗せた。  
たとえば、DDDは正式には単一階層システムと呼ばれているものと見なすことができます。  
DDDはコーディング時と実行時の概念を曖昧にしているように見えます（良いことです）が、境界のあるコンテキストの単一構造の背後にある1つの観点と哲学があります。  
問題はそれらが制限されているということです。  
現実の境界が現実の世界に存在することはめったにありません。  
経理部門とUXデザイナーは、明確なメモやプロトコル、あるいは文書や構造化された会議でさえも通信しませんが、コーヒーメーカーに関する最も重要な市場ニーズを交換するかもしれません。  
彼らのソフトウェア成果物のプロトコルも同様に多孔質であるべきです。


---
ここには他の土地からの光があります。  
私は、優れたドメイン分析と呼ぶものでさえも構築することによって、テレコムやファイナンスなどの成熟したドメインで多くの製品が成長しているのを見ました。  
しかし、ドメイン知識をデザインに留めるための方法に頼るのではなく、これらの製品は、ビジネスと過去の慣習の両方のドメインのパターンを詳しく調べました。  
熟練したテレコム開発者は、システムがコールオブジェクトを機能させるのが愚かであることを知っています（システムは代わりにハーフコールを使用する場合があります - 重要なドメイン知識の洞察）。  
そして、Ericの研究は、DDDが時代を超越したソフトウェア構築の構造を想起させる程度までその光を垣間見ることができます。  
それに問題はありません。  
多くのEricの考えと同様に、問題はプログラマがEricのパターンでビジネスドメインパターンの重要な知識に取って代わることかもしれません。  
Domain-Driven Designでは、半分電話をかけることはできません。  
本の中で見つけたものは、1つのレンガを別のものの上に置くというテクニックを持った施設が役に立つという意味で役に立ちます。  
 大部分の読者は、これらの考えがパターンとして投げかけられるのを見て、大聖堂を建てるのに十分であると彼らの立証を外挿します。  

---
要約すると、百合を金色にすることは2つの方法で失敗します。  
エリックは私達が私達が造っているものより身長の壮大さに道具や方法を膨らませるべきでないことに同意する最初の人になるでしょう。  
それでも、私は多くのDDDショップが、彼らがサービスを提供しているビジネスの語彙の代わりにDDD語彙またはプログラマー語彙のいずれかを使用しているのを見つけます（皮肉なことです）。  
一方、最も成熟したドメインでも、コード化できるという点で複雑さがないとは思わないでください。  
Ne quid nimis.(ラテン語で「過剰なものは何もない」という意味)  
---


## Bring Back Analysis

アジャイルの出現と共に、残念ながら、私は「緑のバー熱」と呼ぶ嫌な形のハッキングの出現を見ました。  
これは、人々が可能な限り最小限のコードに変更を加え、テストを再実行してGreen Barを祈るという、迅速なフィードバックのパブロフサイクルに基づいています。  
何らかの理由でテストがスマートピルを飲んだときに書かれているのに対し、コードが書かれていないときに書かれているかのように、彼らはテストよりもコードを微調整しています。  


---
コンピュータが高速化し、ほとんどすべてのプログラマが膝の上に少なくとも1台の高性能マシンを置いているため、自動化の機会が増えています。  
大野太一からElon Muskまでの優れたデザイン思想家は、あまりにも多くのオートメーションの悪に対して警告しています、
そしてオートメーションが品質を下げそして手直しを増やすかもしれないという事実を支持するたくさんのデータとモデルがあります。  
トヨタが組立ラインからロボットを取り除くにつれて、ソフトウェアエンジニアはますます多くの作業を自動化しています。  
新しいミレニアムの道具と技術は、1950年代から1960年代にかけて、私たち全員が数年以内に自分たちのために食事を調理することを想像したときに、その技術が持っていた名声を受け始めています  

---

DDDは明白な方法でこの罠に陥ることはありませんが、それはほとんど同じ空間にいると理解されるようになりました。 
分析というよりはデザインが重要です。  
私は現在新しい家を建てています。  
サイトを選ぶには何年もかかります。  
敷地内に家をレイアウトするのに数週間または数ヶ月かかります。  
間取り図を選択して建築家と同居するのは数週間かかります。  
家電製品や材料を選択するのはかなり時間がかかります。  
家自体 - 丈夫な、ノルウェー設計のTrelleborgログハウス - は数日で上がります。  
代わりにソフトウェア関係者は分析を完全に捨てて（DDDは分析の活動の余地がないことを明示的に示しています）、設計に取り掛かります。 

---
私の考えでは、ソフトウェアは十分にソフトで言語は十分に表現力があるので、実装の中で思考プロセスを繰り返すことができます。  
経験からの経験、そして私たちの語彙に「技術的負債」という語句があるという単なる事実は、この見方の愚かさを証明しています。  
具体的になりたい人を支援するための実行可能な「ツール」があります。プロトタイピング、セットベースのデザイン、モデリング、形式分析、そしてその他多数のものです。  
これらのことは、Java、Python、またはRubyの快適な領域からオタクを取り除きます。  
だから彼らはコードの中にいます。  
そして彼らは彼らを元気づけるDDDのイメージを作り上げました。  

---

プログラミング言語とその設計方法は、広い意味でのドメイン固有言語の場合を除いて、エンドユーザーのニーズにほとんど洞察をもたらしません。  
むしろ、上記のように狭義の意味を持ちます。  
新たなDDDの展示会では、すでに存在している優れた設計手法の仲間として、健全な分析の場所、または少なくともドメインの専門知識を認めておくことをお勧めします。  


---
先に述べたように、DDDはオタク天国であり、このアプローチはオタクの世界観に役立ちますが、それはエンドユーザーを寒さの中に残します。  
DDDの歴史に大きな悲劇があるとすれば、何十年も前からのドメイン分析の遺産として行われてきたように、ビジネス用語を祝う代わりに、過度に低レベルの構成要素にその言語の概念が誤用されてきたということです。  
それはGuy SteeleがOOPSLAで言語表現の粒度について与えた基調講演を思い出させます。  
彼の話はまた言語についてでした。彼の場合、それはたまたまJavaでした。  
私は同じ批判が1つのより高いレベルのデザイン談話にもあてはまるかもしれないと思います、そして、我々はその問題をDDDで見つけます。  
全体が欠けていて、そしてRebecca Wirfs-Brockが言ったように、オブジェクト指向のデザインは単なるオブジェクトの袋以上のものです。

---
## By, of, and for the people

私は、人々が工場の床の機械のメンテナンスに役立つソフトウェアについて話していたDDD会議のワークショップセッションに行きました。  
私は古いテストを適用することにしました。  
私は座って静かに彼らの会話を聞き、彼らがどんなビジネスに従事しているのかを知るのにどれくらい時間がかかるかを観察しました。  
彼らはユビキタス言語について話し合っていたので、私は思いました：これは簡単なはずです、私は聞きました。  
構成要素（モーター、ベルト、ベアリングアセンブリ）と関連付け（機械を接続するパイプ、チューブ、およびワイヤ）を含むエンティティ（私が考え出したものは機械のようなもの）、
そして結局私がやらなければならなかった他の多くのオタク中心概念についてこれらのマシンが実際に何を作ったのか尋ねてください。  
しかし、モータ、ワイヤ、および特定の機械は、あたかもそのような使用が何らかの理由で設計上の理解を損なうか、または駄目にするかのように通過することにおいてのみ言及された。  
分析なしのデザインでした。  
それが十分な考えなしでデザインであったと言うことはそこから遠く離れたジャンプではありません。  

---

数ヵ月後、私は中国に行き、DDDについて助言を求めているクライアントに奉仕しました。  
彼らはエリックに連絡を取ったが、エリックは本当に中国に旅行したくないと言ったと私に言った。  
それに加えて、彼は自分がそこにいる必要はないという十分な知識を伝えた本を書いた。  
私は何時間ものPowerPoint®によるデザインのUML図のプレゼンテーションを見てきました。  
クラス、クラス階層、そしてアソシエーションです。  
ほとんどの労働者は、数ヶ月または時折、数年の経験を持つ20代でした。  
市場を征服し、ドメインモデル（すなわち、ビジネスドメインの列挙およびそれらの関係の理解）を作成するための協調的な努力はなかった。  
彼らは彼らがどんな問題を解決しているか私に言うことができませんでした。  
オタク天国でした。  

---

分析作業を行うことは、指を汚すことと実社会の階層的でない乱雑さを理解すること、というホイ - ポロイと混ざることを意味します。  
ＤＤＤ構造は、完全な対称性を有する階層（あるいは、せいぜい有向非巡回グラフ）である。  
その対称性はそれに優雅さを与えます、そしてその優雅さは分析的な心に訴えます。  
私たちの心は、おおよその自然の対称性を使って、記憶がどのように機能するのか、エネルギーを節約するのかを欺いています。  
ただし、自分の写真を注意深く分析すると、自分は対称的ではないと感じるでしょう。  
（顔を真っ直ぐに撮り、2枚コピーし、各コピーを完全に半分に切って、鼻のすぐ下に置いてください。あなたの多くの版を見るためにさまざまな方法で半分をまとめてください。）  
それでも建築家のChristopher Alexanderは、美は対称性の破れと、避けられない自然の不完全性との調和によるものであることを私たちに思い出させます。  
Jef Raskin（Humane Interfaces）のような多くの人が、人間の脆弱性や誤りに強いソフトウェアを作成するように私たちに勧めています。  

---

## Mental Models

私にとってマイナスの1つは、DDDは人々についてはほとんど話していないということです。  
今日のほとんどのソフトウェアはエンドユーザーと対話しています。そのためには、基盤となるソフトウェア構造、ヒューマンインターフェイスの要素、およびエンドユーザーのメンタルモデルをうまく調整することが重要です。  
DDDはオタクの復讐のようで、機械の中に座っていて、人間に邪魔されていません。

---
メンタルモデルが方向性のあるコンテキストをどのように作成するかを直接的に推進することができれば、バグが少なく、より良く進化し、そして理解しやすいシステムで終わることになると思います。  
これらの懸念は、プログラミング言語で、あるいは新しい意味でのDSLでさえ表現できる設計上の考慮からはほど遠いことが多い。  
それらは、プログラミング言語の選択さえもずっと前から行われている分析とモデル構築の問題です。  

---
私が建てている新しい家は海に近い砂丘の中にあります。  
私達は彼らのレイアウトがどのように通常の猛烈な天候と時折の砂嵐に対処するかについてその地域で家を建てた多くの人たちに話をしました。基礎が砂と芝の層の土でどのように機能するか。  
その地域が世界的に有名な、信じられないほどユニークな光をどう利用するかなど。  
家の間取り図を見ているだけではなく、広くて掃除が簡単なものを選んで、私たちの敷地に配置しました。  
私は無人機を買いました、そして我々は空中調査をしました。  
私たちはたくさんのレイアウトをいくつか試作しました。  
これらのことのどれも、建築家の絵や彼の製図ツールから来たものではなかったでしょう。  
そしてそれはソフトウェアにあります。  
システム全体の形式とその部分の設計をユーザーのメンタルモデルに結び付けることが重要です。  
DDDはオブジェクトについて語っています。  
エンドユーザーのメンタルモデルをソフトウェアに取り込むことが、オブジェクト指向が作成された全体の理由です。  
DDDはパターンについて語っています。  
住人の住人の内なる感覚に本能を合わせさせ、デザインを駆り立てることが、アレクサンドリア全体のアジェンダです。  

---

## Break the Symmetry


DDD会議で、DCIと呼ばれるオブジェクト指向プログラミングのルネッサンスについて話しました。  
データ、コンテキスト、インタラクションのパラダイム  
それは彼が何年も前にオブジェクト指向と名付けたものの下にあるアラン・ケイの基本的な考えに戻ることを試みた。  
アランの世界は子供たちの精神的モデルと世界の表象の世界でした。  
それは乱雑な世界です。  
物事は必ずしも高度に結合されたデータと方法のきちんとしたカプセル化にうまく収まるとは限りません。  
そのような遺伝子座（オブジェクトと呼ばれる）は便利な近似ですが、全体の物語はそれらの間の相互作用のネットワークで展開します。  
そしてそれこそが価値のあるところです。  

---

ケイの世界では、これらの相互作用のいくつかは、オブジェクトがコラボレーションする機会を見つけたときにオンザフライで行われます。他のものは、たとえばユースケースとして設計できます。  
DCIでは明らかに後者に焦点を当てています。  
どちらの場合も、焦点はオブジェクトとその相互作用にあります。  
相互作用するオブジェクトが存在します。  
クラスは、あなたの思考を限界のある計算領域に限定するために存在します。  
それ自体では意味がありませんが、エンジニアが推論できるような方法で計算が展開される単なる状況です。  
それらを有界文脈と呼ぶかもしれず、そして認識の観点から、クラスとDDDの適切に命名された有界文脈はこの特性を共有する。  
それらは首尾一貫した世界観、すなわち自己完結型の首尾一貫性を持つ首尾一貫した語彙の軌跡です。  


---

DDDはその中心に階層を持っています。  
これには、次のような意味があります。  
特定のドメイン（アプリケーションまたはデザイン談話の領域）は、コード内で表現を見つけられない可能性がありますが、実際には複数の有界コンテキストにまたがる可能性があります。  
つまり、ドメインの変更を推論するためには、DDDで境界のあるコンテキストとモジュールを分離する方法がないように思われるため、複数のモジュールに対する調整された変更が必要になります。  
これは、もちろん、結合と結束の重要性についての半世紀前の知恵に反するものです。  

---
DCIの（限定された）コンテキストはユースケースです。  
エンドユーザーのメンタルモデルから運用モデルを反映した計算を実行する機会が生じるように設定できるネットワークオブジェクトです。  
オブジェクトはいくつかのそのようなコンテキストに参加するかもしれません。  
クラスには、このようなつながりや、より大きな全体に属するという概念が欠けています。  
そして、同じことが境界のある文脈にも当てはまります。  

---

DCIはまた、そのようなドメインの考慮事項によってソフトウェアを分類することもできます。  
それはまさにこれをすることにおいて長年の地位を持っているクラスを使うだけです。 
オブジェクト間の動的な関係は、ある意味で別の次元にあります。  
さらに別の側面では、運用モデル内で互換的に機能することができるドメイン内の一連の細分化があることがわかりました。  
実際のソフトウェア設計は複雑であり、設計はそれがアプリケーションに存在するのと同じくらい多くの次元を表現することができる程度に洗練されそして維持可能である。  
ソフトウェアのアーキテクチャーと設計における大きな進歩を見れば、それらはどれほど上手に複数の対称性を表現できるかということでした。  
側面は複数の対称度を表現しようとしましたが、洗練されていませんでした。  
C ++、Ruby、およびC＃はすべて、なんらかの面倒な言語であり、さまざまなソフトウェア形式を表現できます。   
Scheme、Lisp、Smalltalkはエレガントに対称的です。  
どの人が生き残ったと思います。  
DCIは壊れた対称性を意識的に豊富に含んでいますが、DDDはほとんど純粋に階層的です。  
基本的に1つの構成要素があります。それは境界コンテキストです。  

---

Ericの本は、説明のための構造としてパターンをよく使用します。  
これは私が理論が次の段階に移行するのに貴重であるかもしれないと信じる1つのケースです。  
パターン理論はすべて私達が作り出すものの間の相互作用と分離しないことについてです。  
アレクサンダー自身はしばしば「分離しない」というフレーズを使用し、描写された近所 - その境界のある文脈に基づいて都市計画を非難する彼のエッセイ「都市は木ではない」で知られています。
DCIは2次元（または3次元）の対称性のみを破るという点で、パターンはDCIを超えています。  
彼らは多数です。  
それらを無視するデザイナーは非人道的なシステムを生み出すでしょう。  
多くの慣用言語構造は対称性の破れの一種です。  
Cで配列をコピーすると、初心者は次のようになります。  

    # Tab
    char array1[10], array2[10];
     . . .
    for (int i = 0; i < 10; i++) {
     array1[i] = array2[1];
    }


---



しかし、それは言語の標準的な文法に準拠した（対称的な）構文とセマンティクスにすぎません。  
複数の言語構造を混在させると、次のようになります。



    # Tab
    char array1[10], array2[10];
     . . .
    char *cp1 = array1, *cp2 = array2;
    while (*cp1++ = *cp2++);


---



表現の真の豊かさは、概念の重複にあります。  
たとえば、フライト予約では、路線と飛行機の種類、したがってサービスクラスとの間に大きな重複があります。  
DDDはそれらを分離しています。  
なぜなら、そのような懸念を表現するためには対称次元が1つしかないため、記述は線形であるためです。  
階層はほとんど線形化以上のものです。  
線形シーケンスには固有の階層がありませんが、すべての階層を固有のシーケンスにマップできます。  
有向グラフ、あるいは有向非巡回グラフ、またはグラフではそれはできません。  
複雑なデザインはグラフです。  
円をスライスするには、おそらく間違いなく正しい方法がたくさんありますが、それでも設計者は1つだけを選択する必要があります。



---

いくつかのDDD概念に基づいて構築できる次世代のDCI、または複数の階層を表現できる次世代のDDDには、大きな可能性があると思います。  
HéctorValdecantosらによる研究のように、それはぶら下がっている実であり、人間のデザインの有効性を助けるように階層をスライスする方法としてすでに証明されています。  
示しています。  
この技術は存在しており、この2つを組み合わせることは大部分が情報に基づいた技術的課題です。

---
## Domain Specific Languages


ユビキタス言語をユビキタスにする必要があります。  
言語には力があり、DDDをデザイン構造の言語学上の最後の単語と見なすと、完璧を追い出してしまうという危険があります。  
実際、DDDは従来の技術と比較してデザイン言語学に対する意欲を過度に薄めており、どちらも可能性のあるものの影となる可能性があります。  
アレキサンダーは彼のパターン形式主義の設計言語の長年の概念を復活させた。  
おそらく、オブジェクト指向の心理学的基盤と一緒に、言語という広い概念をテクノロジーの前に持ってくる方法についての洞察の新たな扉を開くことができます。  
統計学者にはS、それぞれの分野にはExcelとyacc、そしてPowerPointがありますが、自動車用ナビゲーションソフトウェアやビデオゲームのデザインのための言語を作成するための基準を引き上げる可能性があります。  
そうすることは、おそらくソフトウェア設計をその基礎の間の快適ゾーンから代数的に置き換えるでしょう。  
ほとんどの言語はまだ代数と代入の基本演算子を持っていますが、これらはヒューマンタスクの自動支援の問題のほとんどとはほとんど関係ありません。  
そのような世界では、設計方法ができることはすべて、識別子の語彙を変調することだけです。ユビキタス言語は、語彙ではなく言語のレベルで、業界としての私達がまだ衰退していないパラダイムシフトです。  
それは刺激的な可能性です。

---

## A Taxonomy of Theory and Heuristics(理論とヒューリスティックの分類)


あまりにも多くのコンピューター科学者は、自分のコードに対して過度に深い合理化または過度に正式な理由を求めています。  
私達はユーザーニーズが死ぬまで分析することができます。  
しかしフロイトが言うように、時々葉巻は単なる葉巻です。  
時には、互いに素な境界のある文脈が単なるチケットです。  
宇宙には他のものから完全に分離されているものは何もありませんが、分離はそれぞれの概念が独自の自己完結型のエンティティを持つことができるほど十分に優れていることがあります。  
そのような分離のための時間と場所があります。  
おそらく最も大規模なレベル（ミサイルナビゲーションソフトウェアをレーダーアンテナの油圧を制御するプログラムから分離する）と最高レベル（Stringはかなり高度な整合性の概念です）。

---
それでも物事はその間に厄介であり、そして対称性は壊れます。  
新しいエンティティをいつ作成するか、DCIなどのより洗練されたアプローチをいつ使用するかを決定するには、ヒューリスティックと設計の両方の形式が必要です。  
時には文化が衰退し、実際には絡み合った概念は人間の精神的なモデルとどのように一致するかに起因してそれ自身のアイデンティティに値するものであるものに値する。  
おそらくそのような状況は、語用論と理解に伴うソフトウェア保守性の力のために、OccamのRazorを脇に追いやらせるでしょう。  
それが理解できないのであれば、本当の物語は無用であり、たとえ誤った物語（寓話、神話）であっても大きな力を伝えます。  


---
## Sendoff

それで、あなたはそれを持っています：私たちのデザインへの共通の願望に関連するアイデア、希望、そして異端の浪費心のダンプ。  
私はそれがあなたの顔に笑顔をもたらし、そしてあなたが今後15年間働くべき何かについて熟考することを願っています。  
ゴッドスピード Neighbors、J.（1984）、 "再利用可能なコンポーネントからソフトウェアを構築するためのDracoのアプローチ"、ソフトウェア工学に関するIEEEトランザクション10、5、564-574。  
SiniaaltoとAbrahamsson。テスト駆動開発はプログラムコードを改善するか憂慮すべき 2007年の議事録2007年、2007年10月10日から12日、ポーランド、ポズナン。
Guy Steele. Crafting a Language, OOPLSA 1998.⁵⁸
James Coplien. Multi-Paradigm Design for C++. Reading, MA: Addison-Wesley, 1998.
Christopher Alexander. “A City is Not a Tree.” In Architecture Forum, Sustasis Foundation, Boston,MA, 1965, ISBN 978-0-98-934697-9.
Angela Martin, R. Biddle and J. Noble. “The XP Customer Role in Practice: Three Case Studies.”
Proceedings of the Second Agile Development Conference, 2004.
Héctor Valdecantos, Katy Tarrit, Mehdi Mirakhorli , and James O. Coplien. “An Empirical Study on Code Comprehension: Data Context Interaction Compared to Classical Object Oriented.”
Proceedings of ICPC 2017, IEEE Press, May 2017.
Taichi Ōno. Toyota production system: Beyond large-scale production. Cambridge, MA: Productivity Press, 1988.
Jef Raskin. The Humane Interface: New Directions for Designing Interactive Systems. Reading, MA:Addison-Wesley, 2000.

---





   


















  