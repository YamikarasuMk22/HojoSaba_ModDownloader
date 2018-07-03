modリスト(json)の説明
	[
		{
			"available": "ダウンロードする:1, しない:その他",
			"name": "modの名称",
			"version": "modの適正バージョン(わかる範囲)(空欄可)",
			"url": "modのダウンロードURL",
			"required": "必須:1, オプション:0",
			"description": "modの説明(簡潔に)(空欄可)"		←※最後はカンマをつけない
		},
		{
			...
		}													←※最後はカンマをつけない
	]

urlについて
	そのまま書いても動きますが、できるだけ以下のように書いてください
	minecraftのバージョン部分 {$m_ver} 「1.7.10」に変換されます。
	Forgeのバージョン部分 {$f_ver} 「10.13.4」に変換されます。
	Forgeのリビジョン部分 {$f_rev} 「1558」に変換されます。
	mod自体のバージョン部分 {$ver} 「versionの値」に変換されます。
	(ビルドクラフト7.1.23)
	例
		・http://sample.com/download/MCTE1.7.10.12_Forge10.13.4.1558.jar
		→http://sample.com/download/MCTE{$ver}_Forge{$f_ver}.{$f_rev}.jar

		※わからん時は数字部分(ハイフン等含む)を全て{$ver}にしちゃってください。
		※{$ver}にした部分をversionに書くのを忘れないようにしてください。