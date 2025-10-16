## How to Write \*ACL Papers

##### Nikos Aletras
##### v1.3 16-10-2025
----


### Main NLP Venues

- Top-tier NLP conferences (\*ACL):
  - ACL, EMNLP, NAACL, EACL, AACL
- \*ACL Journals:
  - TACL, Computational Linguistics
- Other top NLP conferences:
  - COLM
- Closely related top-tier venues:
  - ML:
    - NeurIPS, ICML, ICLR
  - General AI:
    - AAAI, KDD
  - Social Media and Computational Social Science:
    - ICWSM
  - Web and Information Retrieval++:
    - SIGIR, WWW, CIKM, WSDM

Acceptance rates: typically ~20-25% for the main proceedings. At \*ACL venues an extra ~15-20% of the rejected papers is accepted to Findings (technically sound papers, perhaps not very novel with borderline scores). See https://aclweb.org/aclwiki/Conference_acceptance_rates. 

Two paper types for \*ACL conferences:
  - Long: 8 pages content + unlimited pages for refs
  - Short: 4 pages content + unlimited pages for refs (Note that recently the acceptance rates for short papers is lower than long papers!)

Usually you get +1 page of content upon acceptance.

Number of submissions in *ACL conferences: ~1-7K (or more).


### Paper Submission and Review Process

- Papers are submitted into different tracks e.g. syntax, semantics, machine translation via ACL ARR.
- Papers are reviewed by three reviewers (sometimes you might receive four reviews if one of the reviewers is late in submitting their review) and a meta-reviewer
- Papers are rated from 1 to 5 (Overall Assessment, Soundness and Excitement). Typically, if you get at least two 4s and a 3 for Overall Assessment, or more with a metareview of 4 or more, you have good chances to get your paper in. High Soundness increases your chances for Fidnings, while high Excitement could increase your chances for main.
- The Area Chair provides a metareview to the conference Senior Area Chairs who make accept/reject (or more precisely for \*ACL conferences: "accept to main", "borderline main", "findings", "borderline findings", "reject") recommendations to the Programme Chairs (upon paper commitment to a particular conference). Program Chairs make the final acceptance decisions.

### How can I get my paper published?

To have good chances to get your paper accepted, it should typically make at least one of the following contributions:
  - a novel task
  - a novel dataset
  - a novel methodology (e.g. new ML model, substantial extensions to existing models etc.)
  - a novel evaluation method (e.g. a better way for evaluating models for an existing task)
  - state-of-the art results (compared to previous work)
 
 You need solid and thorough experiments, in-depth analysis, and…it has to be **written very well**!

## General Advice

- Start writing early
- Keep the sentences (paragraphs) short (brief) and concise
- Use simple language
- Tell a nice story
- Highlight the important results, offer an in-depth and convincing analysis
- **Convince** the reviewers that your paper presents a useful/important contribution for the NLP community!


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

To save space, you can move hyperparameter tuning info into an Appendix


### Abstract
It should start with a sentence setting the context and why the task is important. Then, it should present the limitations of previous work (if applicable) followed with what new you are proposing. Close with the main contributions of the paper. 

Example 1:

*X is an important task in natural language processing with applications in Y and Z. Previous work on X has focused on using A and B however these approaches lack of D and F. In this paper, we present a new method C that consists of two steps: (a) M that includes...; and (b) N that does...Evaluating C on a set of standard datasets, we show that it outperforms previous methods by a large margin. We also show that C is robust in K by experimenting with D and F.*

Example 2:

*A is X used to do Y and Z. It is useful for B and C. In this paper, we present the first computational study of A. We introduce a new publicly available data set of.... We run a battery of supervised machine learning models for automatically detecting A. Our results show that A can be predicted with an accuracy up to K%. Finally, we identify the markers of A through a linguistic analysis.*


### Introduction

The introduction should clearly set the scene, convincing the reader/reviewer that this paper is worth accepting/reading. Typically, its length should not be longer than 1 1/2 for long papers and 1 page for short papers.

The **first one or two paragraphs** of the introduction should provide the context and motivation followed by why the task is important or useful for NLP research (e.g. downstream applications).

<!-- Example:

*  -->

The **second (or third) paragraph** should describe what has been done before (previous work) and its limitations (if any). Note that this paragraph might be longer if the paper is short and does not contain a "Related Work" section. Tip: the limitations of the previous work are often the methodological contributions of your paper rephrased!

The **fourth (or fifth) paragraph** should describe shortly and concisely what you do in your paper.

Example:

*In this paper, we present a new method X that consists of A and B...*

In the **last paragraph**, you should describe (again) shortly and concisely the **main contributions** of your paper. In a long paper, you can use a bullet-point list. For short papers you can use an in-line list (e.g. (a) contribution 1; (b) contribution 2...).

Note: Do not use "The paper is structured as follows…" to close the introduction! This is usually helpful for longer documents such as a PhD thesis.  

### Related Work

In this section you need to list and discuss previous/related work by highlighting its limitations and differences to your own work. Try to group related work in paragraphs and subsections based on their topic or the methods that they use.

### Methodology (or Models)

In this section, you should describe your methodology. Typically, this section usually describes predictive models (in an empirical study of a task) or a new model that you present. Note that you should group your methods into relevant subsections or use a subsection for each method. You should also make sure that your notation is clear and the names of the methods are consistent across sections (typically you will use the names of the methods to describe the results). Make sure that the order of the methods is the same as in your main table of results (see Results). Avoid describing hyperparameter choices here (only rarely in short papers if this is not a lot due to space constraints).

### Experimental Setup

This section should describe hyperparams, baselines, datasets and evaluation metrics each in a subsection or named paragraph. If there is no space, hyperparam description can be moved into an appendix. Baselines description should be short and follow a similar format to the Models/Methodology section.

### Results

This section should critically discuss the main results/findings. Typically when you should test for statistical significance or report results over multiple runs with standard deviation. You should always try to justify observations and if possible link to any assumptions you make or related work. Note that you should provide comparative results and do not forget to include numbers (and relative differences) in the discussion. Try to group the discussion of the results similar to groups you have in your results table (if any).

Example:

*Overall, we observe that transormer-based methods outperform recurrent architectures. The best transformer method X achieves 75 F1 compared to 70 of the recurrent method Y. This happens because...*

Finally, an "Error Analysis" subsection is very important and should highlight and provide explanations for cases where the best performing method fails to classify correctly.

### Conclusion

The conclusions section should be short and reiterate through the main contributions. Tip: rephrase the last paragaph of the intro (or the abstract) and add a couple of sentences on future work.


### Data (if applicable)
If your paper presents a new dataset, then you should include a dedicated section after Related Work. In this section, you need to describe clearly and in detail the data collection/curation/annotation methods. You should include detailed dataset statistics (with relevant tables or plots). If the dataset includes human annotation, you need to report inter-annotator aggreement, instructions to annotators etc..


### References

- Make sure that the format of the references is correct and capitalisation is OK. Always use bibtex.
- Cite the published version of the paper instead of the arxiv version when possible.


## Improving Paper Clarity

- Equations should be well defined and explained in the text.
- Tables/Figures should be well placed/formatted.
- Captions should be short, concise and self-contained if possible.
- Figures/graphs/tables and any text within should be clear and visible.
- Make sure you use colourblind-friendly colour palettes in figures, plots, tables etc.. 
- Latex source should be correct. Use oficcial templates. Never compile an appendix with the main paper (unless this is allowed).
- Bibliography format should be clean and well formatted.
- Place footnotes after punctuation marks (. or ,), e.g, ...end of sentence.\footnote{...}
- In general everything in the paper should be clearly explained. If something looks difficult to comprehend then you might need to revise it.
- Polish, proofread, repeat. Read the paper again and again.
- Ask your colleagues for feedback, ask GenAI for feedback.
- Make sure you have checked any extra requirements (e.g. ethics statement, limitations). Always read carefully the instructions in the official call for papers.
- Use GenAI to fix typos, awkward syntax, and grammar. You can use it on the sentence, paragraph or (sub)section level to get suggestions on different levels of granularity.
- If you use GenAI for writing assistance:
    - Beware LLMs hallucinate. Always double check and post-edit the text.
    - Make sure you clean up "GenAIisms" such as delve, meticulous, significant (without providing statistical significance tests), "quoted text,"-> "quoted text" etc..

## Improving your Writing

- Practice...a lot!
- Have a reading routine by blocking time to read every week. Typically, try to read a good number of papers (https://aclweb.org/anthology/ and arxiv)
- Learn from the best: read papers, paper introductions from researchers that publish frequently in \*ACL. Try to be critical with the structure, paper style and presentation of papers you read. Previous work can help structure your own paper too!
- Write your own papers.
- Ask for feedback.
- Follow academic writing tips, e.g. http://www.cs.joensuu.fi/pages/whamalai/sciwri/sciwri.pdf
- Attend and present at the reading group!
- Non-native EN speakers have to try harder than native speakers! Check for grammar/syntax structure (I personally do web look ups, now you can use LLMs), watch films/series using English subtitles.

