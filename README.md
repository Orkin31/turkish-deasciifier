# deasciifier: Turkish deasciifier

This is a deasciifier for Turkish. It takes a Turkish string containing only
ASCII characters and replaces the relevant characters with their corresponding
Turkish letters.

This system is based on the [turkish-mode](http://github.com/emres/turkish-mode)
by Deniz Yüret.

Example library usage:

		import Deasciifier

		my_ascii_turkish_txt = "Opusmegi cagristiran catirtilar."
		deasciifier = Deasciifier(my_ascii_turkish_txt.decode("utf-8"))
		my_deasciified_turkish_txt = deasciifier.convert_to_turkish()
		print my_deasciified_turkish_txt.encode("utf-8")

Example command line usage:

		$ echo "Opusmegi cagristiran catirtilar." | python deasciify
		$ cat somefile.txt | python deasciify
