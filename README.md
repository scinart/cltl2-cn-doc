## This is an attempt to translate cltl2 into Mandarin

I'm no familiar with tex so I choose the html version.

任何我能力之外的地方我都用四个`.`标出来了。
用``grep -r "\.\.\.\." --include="*.html" ./``就可以看见

All files but .html files are ignored. You should get a complete version from http://www.cs.cmu.edu/afs/cs.cmu.edu/project/ai-repository/ai/lang/lisp/doc/cltl/cltl_ht.tgz
then you can replace origin html files with the modified files here.

Basically what you need to do is the following:

	git clone git@github.com:scinart/cltl2-cn-doc.git
	cd cltl2-cn-doc
	wget -v http://www.cs.cmu.edu/afs/cs.cmu.edu/project/ai-repository/ai/lang/lisp/doc/cltl/cltl_ht.tgz
	tar -zxvf cltl_ht.tgz
	/bin/cp -r --no-clobber cltl/* ./
	/bin/rm -r cltl


Other versions can be reached from http://www.cs.cmu.edu/Groups/AI/html/cltl/cltl2.html

This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.
http://creativecommons.org/licenses/by-nc-sa/4.0/deed.en_US
