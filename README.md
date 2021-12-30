# West Lombard (Milanese dialect)

## About the dataset
The texts represent Wikipedia articles in the Lombard language. First, the metadata was obtained via PetScan, after which 200 longest texts were collected using Wikipedia API. We only included articles that were labeled with both "Articol in Milanes" and "Articol in ortografia milanesa". Finally, we manually discarded articles that contained mathematical formulas or descriptions of geographical objects of the same type and deleted titles and bibliographical references from the remaining texts. We ended up with a total of 54 texts, 4142 sentences, and about 135 000 tokens. The first 1 650 sentences were evenly distributed between 11 annotators (150 sentences in each file), and every annotator chose at least 50 sentences as they saw fit.

## Files
* *milanes_lombard_auto.conllu* -- the full dataset (54 texts, 4142 sentences, ~135 000 tokens) annotated automatically via [UDPipe 2.6 web](http://lindat.mff.cuni.cz/services/udpipe/run.php) (model [italian-isdt-ud-2.6-200830](https://github.com/UniversalDependencies/UD_Italian-ISDT))
* *milanes_plain_text.txt* -- the full dataset in plain-text format (after preprocessing)
* *milanes_X_Y_annotator_Z.connlu* -- files with the annotated sentences (*X* and *Y* -- ids of the first and last sentences, respectively; *Z* -- the total number of sentences annotated by *annotator*)
* [parsing_milanese_wiki](https://colab.research.google.com/drive/1IIMp8-U9cSzSlYFikL9oXx_jNcnOyVdf?usp=sharing) -- a Google Colab notebook scraping Wikipedia articles in Lombard
* [cleaning_milanese_dataset](https://colab.research.google.com/drive/1P1ZdEXQ68xL5IrjMFvhJuuVxfQ62y6Q3?usp=sharing) -- a Google Colab notebook cleaning the dataset  

## Bibliography & References
C. Beretta. Grammatica del dialetto milanese. 1998.
[Dizionario dei dialetti (Dialettando.com)](https://www.dialettando.com/dizionario/dizionario.lasso)
[Ломбардско-итальянский словарь (Glosbe)](https://glosbe.com/lmo/it)
