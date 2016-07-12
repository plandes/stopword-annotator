Stopword Plugin
===============
This is an extension to the
[Stanford CoreNLP analytics pipeline](http://stanfordnlp.github.io/CoreNLP/) to
check if a token's word and lemma value are stopwords.

Fork
----
This is originally John Conwell's
[coreNlp](https://github.com/jconwell/coreNlp) extensions library.  I've
updated the dependencies in the POM and only kept the stopword plugin and
changed the packing so I can deploy it to Maven Central (under my account).

Identifying Stopwords in CoreNlp
--------------------------------
By default, the StopwordAnnotator uses the built in Lucene stopword list, but
you have to option to pass in a custom list of stopwords for it to use instead.
You can also specify if the StopwordAnnotator should check the lemma of the
token against the stopword list or not.

For examples of how to use the StopwordAnnotator, take a look at
StopwordAnnotatorTest.java

Authors
-------
John Conwell (original author)
Paul Landes
