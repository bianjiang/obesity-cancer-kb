# Towards an Obesity-Cancer Knowledge Base

This repo initially contains the data we used to evaluate our biomedical named-entity recognition (NER) and relation extraction methods for automatic construction of a obesity-cancer knowledge base.

* 2017-04-28: We are currently building the pipeline for the construction of the obesity-cancer knowledge base. Coming soon...

2017
--

> Lossio-Ventura JA, Hogan WR, Modave F, Hicks A, Guo Y, He Z, Vasconcelos M, Bian J*. Automatic construction of an obesity and cancer knowledge base from biomedical literature. Under Review.

Compared with our previous work, we added methods for predicate extraction and relation classification. Now, with all the necessary pieces, we have a complete pipeline for automatic construction of a semantic web knowledge base from biomedical literature. Further, to make our biomedical NER and predicate extraction methods more robust, we have annotated a significant amount of additional Pubmed abstracts, and extracted more training data (694 annotations vs. 462 annotations in our previous publication).

*Dataset*

[ObesityCancerAnnotatedPubMedAbstracts_042017.csv](data/ObesityCancerAnnotatedPubMedAbstracts_042017.csv)

*Abstract*

Background: There is a significant association between excess weight and a variety of cancers and chronic conditions, likely mediated by inflammation. Nevertheless, the information available on the Internet, as it pertains to the links between cancer and obesity remains overall of insufficient quality to help Internet users make informed decisions. Patient empowerment has the potential to drastically improve health outcomes. Therefore, it is critical to address the lack of quality health information on the association between cancer and obesity. A formal knowledge representation would help better organize and deliver reliable and accurate health information that the consumers need.  Currently, there are several efforts in the biomedical and life science to convert unstructured data to structured data (e.g., semantic web knowledge base).  However, the development of appropriate tools, e.g. analytics methods and ontologies that are obesity and cancer specific, are important to guide the knowledge base construction process, which ultimately will empower patients and subsequently improve their health outcomes.

Methods: We developed a framework to curate an obesity and cancer knowledge base from PubMed abstracts, based on tools stemming from both machine learning (ML) and natural language processing (NLP).  It consists of four steps: (1) a biomedical named-entity recognition (NER) approach tailored to identify domain specific terms, especially those that cannot be found in existing terminologies and ontologies, (2) a predicate extraction method that leverages statistical and linguistic patterns to identify predicates from a sentence, (3) a relation detection module that detects if two entities and a predicate form a valid relation), and finally (4) a relation classification component that categorizes a predicate into one of 12 relation classes derived from the Relation Ontology (RO). 

Results: The 4 steps of the framework were evaluated separately.  We used two datasets to evaluate the proposed biomedical NER approach: (1) we identified 23 abstracts related to obesity and cancer in PubMed, and manually annotated 214 sentences from the selected abstract to generate a first gold-standard dataset; (2) the second dataset we selected is the National Center for Biotechnology Information (NCBI) disease corpus with annotated mentions and concepts. Our method outperformed a number of popular biomedical NER tools with an F-measure of $90.1\%$.  We then used our manually curated gold-standard PubMed abstract dataset to evaluate the other 3 components: predication extraction, relation detection, and relation classification.  We compared the performance of our predicate extraction method to a state-of-the-art application obtaining a significant better F-measure of $51.8\%$.  Our relation detection method obtained an F-measure of $98.6\%$.  Finally, the multi-class classification model achieved an F-measure of $85.3\%$ when we classified the specific relations to RO classes. 

Conclusions: We have developed a framework for building an obesity and cancer knowledge base.  The 4 steps in the proposed framework are essential elements in automatic construction of a semantic web knowledge base from large, free-text datasets.  Our initial testing of the proposed framework shows promising results.  Even though we focused on obesity and cancer in this paper, the proposed framework can be easily adapted to other disease domains.


2016
--

> Lossio-Ventura JA, Hogan WR, Modave F, Hicks A, Hanna J, Guo Y, He Z, Bian J*. Towards an obesity-cancer knowledge base: biomedical entity identification and relation detection. Proc of the 2016 IEEE International Conference on Bioinformatics and Biomedicine (BIBM'16). 2016;2016:1081-1088. doi: 10.1109/BIBM.2016.7822672.

*Dataset*

[ObesityCancerRelationDetectionPubmedDataset.csv](data/ObesityCancerRelationDetectionPubmedDataset.csv)

*Abstract*

Obesity is associated with increased risks of various types of cancer, as well as a wide range of other chronic diseases.  On the other hand, access to health information activates patient participation, and improve their health outcomes.  However, existing online information on obesity and its relationship to cancer is heterogeneous ranging from pre-clinical models and case studies to mere hypothesis-based scientific arguments.  A formal knowledge representation (i.e., a semantic knowledge base) would help better organizing and delivering quality health information related to obesity and cancer that consumers need.  Nevertheless, current ontologies describing obesity, cancer and related entities are not designed to guide automatic knowledge base construction from heterogeneous information sources. Thus, in this paper, we present methods for named-entity recognition (NER) to extract biomedical entities from scholarly articles and for detecting if two biomedical entities are related, with the long term goal of building a obesity-cancer knowledge base. We leverage both linguistic and statistical approaches in the NER task, which supersedes the state-of-the-art results. Further, based on statistical features extracted from the sentences, our method for relation detection obtains an accuracy of 99.3% and a f-measure of 99.3%. 
