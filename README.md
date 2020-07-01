## Writing Papers for \*ACL

##### Nikos Aletras
##### 30-6-2020
----

### Main NLP Venues

- Top-tier NLP conferences (\*ACL):
  - ACL, EMNLP, NAACL, EACL, AACL
- \*ACL Journals:
  - TACL, Computational Linguistics
- Other good NLP conferences:
  - COLING
- Closely related top-tier venues:
  - ML:
    - NeurIPS, ICML, ICLR
  - General AI:
    - AAAI, IJCAI, KDD
  - Social Media:
    - WWW, ICWSM
  - Information Retrieval:
   - SIGIR, CIKM, WSDM, ECIR

Acceptance rates: ~20-25%  (See https://aclweb.org/aclwiki/Conference_acceptance_rates)

Two paper types for \*ACL conferences:
  - Long: 8 pages content + unlimited pages for refs
  - Short: 4 pages content + unlimited pages for refs

Usually you get +1 page of content upon acceptance.

Note that recently acceptance rates for short papers is lower than long papers!

Number of submissions in these conferences: ~1-3K



### Paper Submission and Review Process

- Papers are submitted into different tracks e.g. syntax, semantics, machine translation
- Papers are reviewed by three reviewers (and usually a meta-reviewer)
- Papers are rated from 1 to 5 (NAACL sometimes uses a 6-point scale). Typically if you get at least two 4s and a 3 you have good chances to get your paper in.
- Area Chairs provide metareviews to Senior Area Chairs who made acceptance/rejection recommendations to the Programme Chairs.

### How can I get my paper published?

To have good chances to get your paper accepted, it should typically contain at least one of the following:
  - a novel task
  - a novel dataset
  - a novel methodology (e.g. new ML model, substantial extensions to existing models etc.)
  - a novel evaluation method (e.g. a better way for evaluating models for an existing task)
  - state-of-the art results
  - thorough experiments

and…it has to be **very well-written**!

### General Advice

- Start writing early
- Keep the sentences (paragraphs) short and concise
- Use simple language
- Tell a nice story
- Highlight the important results
- CONVINCE the reviewers that your paper should be accepted!


## Structuring your Paper

Typically a long paper should consist of the following sections:

- Abstract
- Introduction
- Related Work
- Methods/Models
- Experimental Setup
- Results
- Conclusion

If you present a new dataset, the section straight after Related Work should describe the data.

If you write a short paper, you can:
  - Merge Introduction and related work
  - Merge Experimental Setup and Results into "Experiments and Results"

To save space, you can move hyperparameter choices etc. into an Appendix


### Abstract
Short version of the introduction. It should start with a sentence setting the context and why the task is important. Then, it should present the limitations of previous work (if applicable) followed with what new you are proposing. Close with the main contributions of the paper.

Example 1:

*X is an important task in natural language processing with applications in Y and Z. Previous work on X has focused on using A and B however these approaches luck of D and F. In this paper, we present a new method C that consists of two steps: (a) M that includes...; and (b) N that does...Evaluating C on a set of standard datasets, we show that it outperforms previous methods by a large margin. We also show that C is robust in K by experimenting with D and F.*

Example 2:

*A is X used to do Y and Z. It is useful for B and C. In this paper, we present the first computational study of A. We introduce a new publicly available data set of.... We run a battery of supervised machine learning models for automatically detecting A. Our results show that A can be predicted with an accuracy up to K%. Finally, we identify the markers of A through a linguistic analysis.*


### Introduction

The introduction should clearly set the scene, convincing the reader/reviewer that this paper is worth accepting/reading. Its length should not be longer than 1 1/4 for long papers and 1 page for short papers.

The **first one or two paragraphs** of the introduction should provide the context and motivation followed by why the task is important or useful for NLP research (e.g. downstream applications).

<!-- Example:

*  -->

Next, the **second (or third) paragraph** should describe what has been done before (previous work) and its limitations (if any of course). Note that this paragraph might be longer if the paper is short and does not contain a "Related Work" section. Tip: the limitations of the previous work are often the methodological contributions of your paper rephrased!

The **fourth (or fifth) paragraph** should describe shortly and concisely what you do in your paper.

Example:

*In this paper, we present a new method X that consists of A and B...*

In the **last paragraph**, you should describe (again) shortly and concisely the main contributions of your paper. In a long paper, you can use a bullet-point list. For short papers you can use an in-line list (e.g. (a) contribution 1; (b) contribution 2...).

Note: Do not use "The paper is structured as follows…" to close the introduction!

### Related Work

In this section you need to list and discuss previous/related work by highlighting its limitations and differences to your own work. Try to group related work in paragraphs and subsections based on their topic or the methods that they use.

### Methodology (or Models)

In this section, you need to describe your methodology. Typically, this section usually describes predictive models (in an empirical study of a task) or a new model that you present. Note that you should group your methods into relevant subsections or use a subsection for each method. You should also make sure that your notation is clear and the names of the methods are consistent across sections (typically you will use the names of the methods to describe the results). Never mention hyperparameter choices here.

### Experimental Setup

This section should describe hyperparams, baselines, datasets and evaluation metrics each in a subsection or named paragraph. If there is no space, hyperparam description can be moved into an appendix. Baselines description should be short and follow a similar format to the Models/Methodology section.

### Results

This section should critically discuss the main results/findings. Typically when you should test for statistical significance or report results over multiple runs with standard deviation. You should always try to justify observations and if possible link to any assumptions you make or related work. Note that you should provide comparative results and do not forget to include numbers (and relative differences) in the discussion. Try to group the discussion of the results similar to the groupings in the results table.

Example:

*Overall, we observe that transormer-based methods outperform recurrent architectures. The best transformer method X achieves 75 F1 compared to 70 of the recurrent method Y. This happens because...*

Finally, Error analysis subsection is very important and should highlight and provide explanations for cases where the best performing method fails to classify correctly.

### Conclusion

The conclusions section should be short and reiterate through the main contributions. Tip: rephrase the last paragaph of the intro (or the abstract) and add a couple of sentences on future work (no need to mention/reveal any groundbreaking ideas here!)


### Data
If your paper presents a new dataset, then you should include a dedicated section after Related Work. In this section, you need to clearly and in detail data collection/curation/annotation methods. You should include detailed dataset statistics (with relevant tables or plots). If the dataset includes human annotation, you need to report inter-annotator aggreement.


### References

Make sure that the format of the references is correct and capitalisation is OK. Always use bibtex.


## Improving Paper Clarity

- Equations should be well defined and explained in the text
- Tables/Figures should be well placed/formatted
- Captions should be short, concise and self-contained if possible
- Figures/graphs should be visible
- Latex source should be correct
- Bibliography format should be clean
- In general everything in the paper should be clearly explained. If something looks difficult to comprehend then you might need to revise it.
- Read the paper again and again

## Improving your Writing

- Practice...a lot!
- Have a reading routine (https://aclweb.org/anthology/)
- Learn from the best: read papers, introductions from researchers that publish frequently in \*ACL
- Write your own papers
- Ask for feedback
- Follow academic writing tips, e.g. http://www.cs.joensuu.fi/pages/whamalai/sciwri/sciwri.pdf
- Attend and present at the reading group!
- Non-native EN speakers have to try harder than native speakers! Check for grammar/syntax structure (I personally do web look ups)
