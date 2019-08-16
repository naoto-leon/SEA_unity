# Sea Unity
use shader graph made Sea 

#### shader graphで海を作った。  

![sea_unity _gif](https://user-images.githubusercontent.com/43961147/63160360-86a31300-c058-11e9-82d8-0d3ee9c47939.gif)


海の表現はshader graphの登竜門的な所があるなと自分的には思っています。  
海に関しては様々なチュートリアルや記事があり、今回作った物はそれらの複合技になります。  

最も手軽な海の表現としてはてテクスチャーのUVスクロールかなと勝手に思っていますが、それだとどうしてもカートゥン調の物になってしまう(そちらもいつか書こうと思います)
ので、今回はリアルな海の表現にこだわりました。  

#### 全体図
<img width="1680" alt="allsea" src="https://user-images.githubusercontent.com/43961147/63167350-04244e80-c06c-11e9-86f0-c38d925439b4.png">

***

#### Texture UV
<img width="1392" alt="simpletexsea" src="https://user-images.githubusercontent.com/43961147/63167489-7432d480-c06c-11e9-8dfa-57de5a11dda3.png">

□基本のUVスクロール。少し特殊なのは向きや速さを変えた二つのTextureをNormalBlendでブレンドしている事。
***

#### Noize
<img width="1207" alt="noizesea" src="https://user-images.githubusercontent.com/43961147/63167791-4c903c00-c06d-11e9-84ba-78206f3326db.png">

□基本的にXとZベクトルしか使わない。(Splitの使い方が違う気もするけど指定した座標を取るやり方を他に知らない(笑))
□とりあえずノイズの動きを作る。(基本的にはVertexで使用したい為)

***
