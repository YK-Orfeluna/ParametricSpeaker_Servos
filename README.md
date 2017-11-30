# ParametricSpeaker_Servos

## 修正事項
ねじ穴をネジの規格に合わせて直径3mmになるように変更（ドリルによる穴あけの負荷を減らすため）<br>
よって，現在のデータを使う場合，Curaで再度GCODEに変換する必要がある

## stl_data
TC102には，このSTL形式のファイルを持っていけば，印刷できます．<br>
ただし，TC102で，各3Dプリンタに合わせた形式のファイルに変換する必要があります．<br>
教室奥の小さな3Dプリンタを使う場合，STL形式で印刷できるようです．

## 123dx_data
3ds Max用のデータです．<br>

拡張子は全て「123dx」です．
## old_data
古いデータです．

## print_data
Curaを使って，3Dプリンタで印刷できるようにデータ形式をSTLからGCODEに変換したものです．<br>
変換時の設定は，印刷速度はFast，マテリアルの充填はSolid（フル充填）です．
### Ultimater_2_Extended+
"Ultimater 2 Extended+"で印刷する時に使用します．<br>
印刷はSDカードを本体に差し込んで，そこからデータを読み込んで行います<br>
所要時間の目安は以下のとおりです．
* micstand:	1h 33m
* param:	2h 26m
* servo_x:	1h 50m
* servo_y:	0h 52m

### Ultimater_3_Extended
"Ultimater 3 Extended"で印刷する時に使用します．<br>
印刷はUSBメモリを本体に差し込んで，そこからデータを読み込んで行います<br>
所要時間の目安は以下のとおりです．
* micstand:	1h 45m
* param:	2h 51m
* servo_x:	2h 07m
* servo_y:	1h 04m