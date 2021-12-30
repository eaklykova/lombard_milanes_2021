# West Lombard (Milanese dialect)

#### This project was conducted by students of the National Research University "Higher School of Economics".

## About the dataset
The dataset consists of Wikipedia articles in the Lombard language.

We started by obtaining the articles metadata via PetScan, after which 200 longest texts were collected using Wikipedia API. Only articles labeled with both "Articol in Milanes" and "Articol in ortografia milanesa" were included in the dataset. We manually discarded articles that consisted mainly of mathematical formulas, descriptions of chimical elements, etc., and deleted titles and bibliographical references from the remaining texts. We ended up with a total of **54 texts, 4142 sentences, or about 135 000 tokens**, which were then automatically annotated with the *italian-isdt* model ([italian-isdt-ud-2.6-200830](https://github.com/UniversalDependencies/UD_Italian-ISDT)) through the [web version of UDPipe 2.6](http://lindat.mff.cuni.cz/services/udpipe/run.php). As the final step, unique ids were added to the sentences; the ids contain information about the language, dialect, and source of the text, as well as the number of text and the number of sentence in the dataset, i.e. *lmo-mil-wiki-doc2-s451*.

The first 1 650 sentences were evenly distributed between 11 annotators, and every annotator chose at least 50 of their 150 sentences to carefully check and correct the automatic annotation, thus creating annotations for the Lombard sentences in a semi-automatic manner. **The total number of manually corrected sentences is 576**, divided into 11 files. The sentences are not necessarily in order.

## Files
* *milanes_lombard_auto.conllu* -- the full dataset (54 texts, 4142 sentences, ~135 000 tokens) annotated automatically via [UDPipe 2.6 web](http://lindat.mff.cuni.cz/services/udpipe/run.php) (model [italian-isdt-ud-2.6-200830](https://github.com/UniversalDependencies/UD_Italian-ISDT))
* *milanes_plain_text.txt* -- the full dataset in plain-text format (after preprocessing)
* *milanes_X_Y_annotator_Z.connlu* -- files with the annotated sentences (*X* and *Y* -- ids of the first and last sentences, respectively; *Z* -- the total number of sentences annotated by *annotator*)
* [parsing_milanese_wiki](https://colab.research.google.com/drive/1IIMp8-U9cSzSlYFikL9oXx_jNcnOyVdf?usp=sharing) -- a Google Colab notebook scraping Wikipedia articles in Lombard
* [cleaning_milanese_dataset](https://colab.research.google.com/drive/1P1ZdEXQ68xL5IrjMFvhJuuVxfQ62y6Q3?usp=sharing) -- a Google Colab notebook cleaning the dataset  

## Annotators
* Veronika Ganeeva
* Yuliya Gorshkova
* Ekaterina Zalivina
* Elizaveta Klykova
* Kseniya Koshkina
* Grigorij Kuznetsov
* Ekaterina Sannikova
* Mikhail Son'kin
* Kseniya Timonova
* Anastasiya Chizhikova
* Zlata Shkut'ko

## Bibliography & References
1. C. Beretta. Grammatica del dialetto milanese. 1998.
2. [Dizionario dei dialetti (Dialettando.com)](https://www.dialettando.com/dizionario/dizionario.lasso)
3. [Ломбардско-итальянский словарь (Glosbe)](https://glosbe.com/lmo/it)


*HSE, Moscow, Russia, December 2021.*
