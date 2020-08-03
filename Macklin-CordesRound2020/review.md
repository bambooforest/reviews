# Review of: "Re-evaluating phoneme frequencies"

* Reviewer: Steven Moran \<steven.moran@uzh.ch\> (August 2, 2020)

* Manuscript title: Re-evaluating phoneme frequencies
* Manuscript ID: 570895
* Authors: Jayden Luke Macklin-Cordes, Erich Ross Round
* Journal: Frontiers in Psychology, section Language Sciences
* Article type: Original Research
* Submitted on: 09 Jun 2020

A preprint of the paper is available on arXiv.org:

* https://arxiv.org/abs/2006.05206

and the paper's supplementary materials are available on Zenodo:

* https://zenodo.org/record/3886212#.XyQzGxMzZGB

An accompaniment to this review is available here (details below):

* https://github.com/bambooforest/reviews/blob/master/Macklin-CordesRound2020/tests.md


## Overview

This paper presents an interesting, and as the authors point out, timely analysis of the frequency distribution of phonemes with the goal of identifying whether or not these distributions follow one, or more, statistical distributions.

The authors argue that identifying the statistical distributions of certain typological linguistic features will help shed light on the potential causal processes underlying these distributions. Identifying causal processes underlying linguistic diversity, it is argued, is an important step in the development of linguistic theory.

The authors take as a case study the phoneme inventories of a large sample of indigenous Australian languages, with the phoneme counts taken from wordlists of 250 or more word types. They then test whether the phoneme frequency distributions in these wordlists fit any of several different statistical distributions.

Whereas the authors point out that such evaluations have historically been done by plotting the frequency of the variable under investigation and by eye-balling whether or not if it looks, for example, Zipfian, or power law like, instead they use more recent state-of-the-art approaches to evaluate phoneme frequencies in terms of statistical distributions, i.e. in a maximum likelihood framework described in Clauset et al., 2009.

I appreciate the authors' honesty regarding the application of the methods to the limited size of their data:

> "This is simply not possible for most of the world’s languages (including all languages in this study) due to the limited size of segment inventories. Thus, in phonemic studies such as ours there is likely to be an unavoidable uncertainty in the estimate of [alpha]."

The authors first fit a power law distribution to the phoneme frequencies in each language, and given the caveat above, they find it is generally a poor fit for the languages in their sample. As they note, previous literature has shown that one-parameter power-law poorly characterizes phoneme frequencies.

Next they fit a power law with the xmin parameter to try to improve the fit of the power law distribution (it removes some of the least frequent observations from the sample). With the xmin parameter, the power law fit is plausible. Nevertheless, the authors suggest that although they cannot rule out the power law distribution, and that it fits better with one parameter, so they investigate several other potential distributions, including log-normal, exponential, and poisson. For log-normal, they cannot confidently rule it out because it fits for around half the languages. For exponential, it seems to be a good fit; however a few languages show a very poor fit. For poisson, the authors find it totally implausible.

The authors then conduct an evaluation for best fit among the multiple plausible distributions by using likelihood ratio tests for model selection. They find that basic power law with a single free parameter is generally insufficient for capturing the frequency distribution of phonemes in languages in their sample. In line with previous work, they find an exponential (geometric) distribution with a single parameter is a plausible fit for (full) phoneme inventories in their sample. They also find that log-normal (with two free parameters) is also a plausible fit. Poisson is not.

Lastly, the authors note that exponential distributions do not fit higher-frequency phonemes as well as power-law and log-normal, but they are a good fit for the entire inventory (which suggests they fit well for the low frequency phonemes). In sum, the authors find that different statistical distributions fit the more versus less frequent portions of the phoneme frequency distributions. (Note that they are not yet able to tell whether power-law or log-normal is a better fit for the higher frequency phonemes.)


## Comments

I find the paper ambitious because its tact is one that can be applied to many different areas of grammar, with the goal of course, to shed light on the causal mechanisms of language change, whether through diachrony or synchrony, by way of leveraging quantitative approaches from statistics and mathematics. Therefore, I found the end a bit disappointing, i.e.:

> "It is beyond the scope of this paper to pursue questions of causation that lie behind the distributions we have uncovered."

Don't the authors have any (at least) speculative remarks (that they are willing to put in print) about the fact that they found phoneme frequencies in languages in their sample are best fit by different statistical distributions -- one for frequent and another for infrequent phonemes? 

The authors note that their findings are:

> "consistent with the observation by Clauset et al. (2009) that, in practice, power laws are rarely observed across the whole distribution—rather, there is a threshold, the xmin parameter, below which the power law ceases to apply"

Why should the frequencies of the full phoneme inventory follow any one particular statistical distribution? This question in and of itself is interesting. 

Given the range of phoneme inventory sizes and the diversity of phonemes on a worldwide scale, should we expect that every spoken language follows the same distribution(s) for the frequencies of use if its phonemes?

Would this not suggest that the diachronic development of phoneme usage and the phonotactics that constrain the combinatorics of consonants and vowels follow some underlying causal mechanisms? Perhaps ease of articulation for the more common phonemes in wordlists?

I think a key issue here is whether the frequencies of consonant and vowel inventories should be evaluated together, as is done in the paper, or if they should be evaluated individually. For example, towards a potential causal factor, Annemarie Verkerk and I have shown that there are differential rates of change in consonant and vowel inventories over time.

* Moran, Steven and Annemarie Verkerk. 2018. Differential rates of change in consonant and vowel systems. In C. Cuskley and M. Flaherty and H. Little and Luke McCrohon and A. Ravignani and T. Verhoef (eds.), The Evolution of Language: Proceedings of the 12th International Conference (EVOLANGXII). April 16-19, Toruń, Poland. DOI: https://doi.org/10.12775/ 3991-1.077. Online: http://evolang.org/torun/proceedings/papertemplate.html?p= 98.

Other work that I am aware of, by Caleb Everett (2018), shows that in wordlists at a global scale, languages show convergence in their use of consonants, i.e. certain consonants share high frequency, whereas other show low frequency, across the board. Everett suggests this may relate to ease of articulation. 

* Everett, Caleb. 2018. The similar rates of occurrence of consonants across the world's languages: A quantitative analysis of phonetically transcribed word lists. Language Sciences, 69, 125-135.

Perhaps also relevant to the authors, Everett (2018, pg. 128) notes:

> "Some consonants are particularly ubiquitous in the word lists, even after controlling for relatedness. There is a power-law association between consonant ranking and frequency, similar though not identical to the Zipfian association well-known to surface in other facets of speech like word usage (Zipf, 1949; Piantadosi, 2015) (The association is technically closer to a Yule-ian association–see Tambovtsev and Martindale (2007))."

I mention here that a potential shortcoming of Everett's analysis, as I understand it, is that he used the relatively small wordlists from the ASJP database (https://asjp.clld.org/). The fact that the authors here used relatively large wordlists (250 or more words) is meant to address any issues regarding estimating the actual frequencies of phonemes in the language.

Personally, in the paper I would discuss earlier why the authors chose a minimum wordlist size of 250, because as I read the paper, I started wondering early on in the Data section why any wordlist data was acceptable for this analysis, given the argumentation by Dockum & Bowern (2019), which is only mentioned at the end.

* Dockum, Rikker & Claire Bowern. 2018. Swadesh lists are not long enough: Drawing phonological generalizations from limited data. In Peter K. Austin (ed.) Language Documentation and Description, vol 16. London: EL Publishing. pp. 35-54. Online: http://www.elpublishing.org/PID/168.

Another argument that the authors could leverage here for using "Australia as an ideal controlled experiment" is that wordlists of a large enough size are not readably available (AFAIK) for a large sample of the world's languages (and if so, they are unlikely to be consistently typologized and orthographically/phonetically normalized). Hence given the impact of wordlist size on phonological generalizations, one arguably should not use a data set like the ASJP for phonological generalizations -- even though as noted above, Everett (2018) reports some interesting results.

One issue I had with the paper was the claim by the authors that:

> "our dataset of phoneme frequencies is very likely to contain the complete population of phonemes in each language"

> "The probability that we have failed to observe some phoneme that exists in a language is small, and even if we did, the missing segment inevitably will be an especially low-frequency type, unlikely to dramatically alter the overall frequency distribution of segments in that language."

However, this claim is not backed up with any analysis in the paper. Instead, I assume it is just presumed given the argumentation by Dockum & Bowern (2019).

Therefore, I decided to test the claim myself in a detailed R markdown report available here:

* https://github.com/bambooforest/reviews/blob/master/Macklin-CordesRound2020/tests.md

The correlation between the number of phonemes as reported in PHOIBLE for the languages that overlap with the phoneme inventory counts as reported in the paper is relatively robust. However, there are clearly some outliers (differences of up to 19 phonemes for two languages) that may be playing a role in the authors' analyses. 

Furthermore, given that the data and the paper are available openly online, I mentioned the issue of correlation to my colleague Nicholas Lester (http://nicholaslester.weebly.com/), who generated a few plots and added some comments that I think the authors may find quite useful. In sum, we highlight what factors influence the variability found in the authors data. For example, lower numbers of segments or lexemes in the authors' data shows greater variability in the difference between PHOIBLE inventories and their data, i.e. smaller samples are less reliable and convergence appears to gain strength around 500 items.

Another question we ask, in regard to comments I made above, is whether consonants or vowels are more or less likely to lead to discrepancies between the counts.


## Minor comments

Nice job on the Shiny app! I do hope you get it hosted online, so that readers can access it without having to load it in R.

Regarding the data, what is the genealogical coverage of these language varieties? Is the sample genealogically balanced within the language families of Australia that it represents? How many are languages and how many are dialects?

I find the following example difficult:

> "Consider for example a so-called preferential attachment process, also known as a Yule process or rich-get-richer process. This can be imagined as having a set of urns, into which balls are added one at a time. Specifically, the urn to which a new ball is added is selected with a probability proportional to the number of balls already in the urn. This simple process has an interesting outcome. Initially, each urn is equally likely to be selected, but the distribution will soon skew, as urns with more balls accumulate additional balls faster than the others. If we rank the urns in terms of which has the most balls, then with time, the relationship between an urn’s rank and how many balls it contains will come to obey a power law."

My recollection of the urn model is that when a ball is selected from the urn, it is replaced to the urn with an additional ball of the same color. Hence, the rich get richer process, because one is skewing the probability by adding more balls of the same color. Something about the above description is lacking, if that's what the author are describing.

The introduction talks about the promise of evaluating and identifying distributions in linguistic phenomena, and below you list a diverse array of phenomena, but you fail to mention what their causal processes are (if it is known).

> "Since Yule’s first demonstration of the link between power law distributions and preferential attachment processes, power laws have been used to characterize the distributions of a diverse array of phenomena in the natural and physical world and in human society (Clauset et al., 2009, 661). City populations (Gabaix, 1999; Levy, 2009; Malevergne et al., 2011), authorship of scientific publications, income distribution (Simon, 1955), the superstar phenomenon in the music industry (Chung and Cox, 1994) and the network topology of the Internet (Faloutsos et al., 1999) are but a few of the phenomena for which power laws have been proposed (see Newman (2005), pp. 327–329 for further examples). And in linguistics, the Zipfian distribution has been used to characterize word frequencies in text corpora (Estoup, 1916; Zipf, 1932,
80 1949)."

It might be worth mentioning the lack of historical agreement on probability distributions of typological variables in general, and that of phoneme inventory sizes in particular. As I wrote in my PhD dissertation (Moran 2012, pg 240):

> "However, there is no agreement on how to measure the underlying probability distribution of typological variables (Cysouw, 2010). For instance, to describe phoneme inventory size, gamma (Lehfeldt, 1975) and log-normal distributions (Justeson and Stephens, 1984) have been proposed. Maddieson (2008a) also hints at a normal distribution (Cysouw, 2010, 30)."

If not, perhaps it is of interest to the authors anyway.


## Typos and suggestions

- "Distribution are properties of variables."

- "article/ supplementary"

- "Macklin-Cordes et al." (* no date)

- "Consequently, if, a variable" (* strange comma placement, for me at least)

- "City populations (Gabaix, 1999; Levy, 2009; Malevergne et al., 2011), authorship of scientific publications, income distribution (Simon, 1955), the superstar phenomenon in the music industry (Chung and Cox, 1994)" (* Is there a missing reference for the authorship of scientific publications?)

- "Consequently, it is important for the development of theory that proposed claims about distributions be as sounds as possible." (* I'm assuming you mean "linguistic theory"?)

- "with negative quantities or zeroes" (* Isn't the plural of zero, zeros?)

- "x might denotes items’ frequencies,"

- "the presence or otherwise of power" (* Strange reading of "otherwise", at least for me.)

- "tightly proscribed range" (*Strange use of proscribed, at least to me.)

- "bootstrapping may indentfy"

- "Using more a reliable evaluation procedure"

- "Our data comes from the Ausphon-Lexicon database, under development by the second author (Author, 2017)" (* I have to say that given the authors are listed on the title page, this isn't very anonymous. :)

Regarding the supplementary materials:

- "S5 is downloadable from https://zenodo.org/record/3886212#.Xt9NFWozaO8."

But clicking on the link in the PDF gives the reader a 404 error (the URL works here).

The supplementary materials that I was able to access contain two data files:

- Aus_metadata_2020-05-21.tsv
- Aus_segment_frequencies_2020-05-21.tsv

First, I think it would be more useful if the authors had a metadata column that specified the Glottolog codes (particularly since ISO 639-3 lacks codes for many Australian languages) than simply the language names. This should not be difficult since most of the languages in the sample are already tagged with a Glottocode in the PHOIBLE database (see accompaniment to this review, which contains the code to do the mapping).

Second, perhaps it's worth noting for the reader why the raw lexical data, phoneme segmentation code, and orthography profiles, used to generate the phoneme frequency counts are not available to the reader in the SI materials or via Zenodo. It seems that some of the lexical data are accessible from the Chirila database, which is freely available after signing the terms of agreement (http://chirila.yale.edu/download). So I assume posting the data openly on the internet is, understandably, not an option. If so, that would be good to know.
