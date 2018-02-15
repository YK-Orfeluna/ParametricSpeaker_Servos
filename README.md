# ParametricSpeaker_Servos
## 注意点
全ての3Dプリンタを同時に利用できるわけではありません．<br>
どの3Dプリンタが稼働中で，どの3Dプリンタを使えるかはわからないので，全ての形式のデータを持っていくことを推奨します．<br>
データはUSBメモリやSDカードに保存して持って行って，備え付けのPCを通して，3Dプリンタ用に用意されたUSBメモリやSDカードに入れます．

## [stl_data](./stl_data)
教室には，この*.stl*形式のファイルを持っていけば，印刷できます．<br>
ただし，各3Dプリンタに合わせた形式のファイルに変換する必要があります．<br>
教室奥の小さな3Dプリンタを使う場合，*.stl*形式のデータから直接印刷できるようです．

### 注意点
上記の「小さな3Dプリンタ」は，__台座へのマテリアルの定着率が低い__，（ガードするものが何もないので）__対流の影響を受ける__といった問題点があり，トライアンドエラーが多数必要になる可能性があります．<br>

## [123dx_data](./123dx_data)
3ds Max用のデータです．<br>
拡張子は全て*.123dx*です．

## [print_data](./print_data)
Ultimaterの3Dプリンタで印刷できるように，データ形式を*.stl*から*.gcode*に変換したものです．<br>
変換時の設定は，印刷速度はFast，マテリアルの充填はSolid（フル充填）です．<br>
__印刷速度を速め__にしているので，出来上がりは荒くなります．<br>
マテリアルをフル充填させているので，印刷時間の増加とマテリアルの使用量の増加，出来上がり作品の重量増加という問題点は生じますが，__出来上がり作品の強度は向上__します．<br>
必要に応じて，印刷速度とマテリアル充填の割合を変更することが可能ですが，その場合は再度*.stl*から*.gcode*への変換を行う必要があります．<br>
つまり，印刷設定を変更する度に，*.stl*から*.gcode*への変換を行う必要があります．<br>
全て，接地面のsupportは有りにしています．

### [Ultimater_2_Extended+](./print_data/Ultimater_2_Extended+)
"Ultimater 2 Extended+"で印刷する時に使用します．<br>
印刷はSDカードを本体に差し込んで，そこからデータを読み込んで行います<br>
所要時間の目安は以下のとおりです．

* micstand:	1h 33m
* param:	2h 17m
* servo_x:	1h 50m
* servo_y:	0h 53m

### [Ultimater_3_Extended](./print_data/Ultimater_3_Extended)
"Ultimater 3 Extended"で印刷する時に使用します．<br>
印刷はUSBメモリを本体に差し込んで，そこからデータを読み込んで行います<br>
所要時間の目安は以下のとおりです．

* [micstand](#micstand):	1h 45m
* param:	2h 48m
* servo_x:	2h 07m
* servo_y:	1h 05m

## 各パーツの解説
### micstand

* servo_yをマイクスタンドに取り付けるためのパーツ
* __回しすぎると，マイクスタンドの雄ねじがこのパーツを貫通__してしまうので注意
* 2つにわかれているので，重ねて使う

### param

* パラメトリックスピーカの超音波照射面に装着するパーツ
* servo_yと合体させる

### servo_y

* y軸方向に回転するサーボモータに装着する
* paramとservo_xとそれぞれ合体させる

### servo_x

* x軸方向に回転するサーボモータに装着する
* micstandとservo_yとそれぞれ合体させる