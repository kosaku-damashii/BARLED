# BARLED
LED Score Bar

aitendoで投げ売りされているLEDを4個使用し、仮装大賞に出てくるような得点板を作成する。
6か所ある表示はそれぞれ3個のLEDで構成されているが、MachiKania type MのI/Oから制御するためにポート数を削減し、端の1個のLEDのみ表示するようにしている。

24点満点で、満点時と23～21点の時と、それ以下の時でそれぞれ別の音声が流れるようにしている。
音声は、
フリーの音声データ(https://soundeffect-lab.info/sound/voice/)を、えこでこツール
(https://ja.osdn.net/projects/ecodecotool/wiki/FrontPage)でWAVへ変換して再生することにする。
なお、音量がSOUNDから出るレベルより小さいので、100dBに設定を変更して変換する。
各音声は下記のファイル名で変換してください。
　「合格です」 "GOKAKU.WAV"
　「おめでとうございます」 "OMEGOZA.WAV"
　「残念でした」 "ZANNENDE.WAV"
　「もう一息です」 "MOUHITO.WAV"
　「不合格です」 "FUGOKAKU.WAV"
　「残念」 "ZANNEN.WAV"
