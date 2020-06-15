## About the Project

![Title Picture](ada2.png)
*<font size="1">Image Credit: Daniel Vorndran, wikimedia commons, CC-BY-SA 4.0</font>*

### Introduction

The study of audio-visual rhetorics of affect scientifically analyzes the influence of auditory and visual staging patterns on the perception of media productions and the conveyed emotions. The AdA project aims to examine the hypothesis of television reports drawing on audio-visual patterns in cinematographic productions to emotionally affect viewers by analyzing television reports, documentaries and genre films of the topos "financial crisis". In a large-scale corpus analysis, film scholars identify and annotate low- to high-level audio-visual patterns, such as shot duration, dominant colors, major-minor tonality and depicted visual concepts. By comparing different annotations from different scenes and genres, film scholars can analyze this opinion-forming level of reporting.

### Goals

The part of the project that is being worked on at the HPI has two main objectives: 1) creation of a standardized annotation vocabulary to be applied for semantic annotations and 2) semi-automatic classification of audio-visual patterns by training models on manually assembled ground truth annotation data. The annotation vocabulary for empirical film studies and semantic annotations of audio-visual material based on Linked Open Data principles enables the publication, reuse, retrieval, and visualization of results from film-analytical methods. Furthermore, automatic analysis of video streams allows to speed up the process of extracting audio-visual patterns.

### Technical Project Setup

The project relies on tool-based video annotations and data management according to the principles of Linked Open Data. [Advene](https://www.advene.org/) was chosen as annotation software for this project because it best meets the needs of film scientists: it offers a timeline view and segment-based annotations of video sequences using multiple tracks that can be used to annotate various aspects under which a video is analyzed. We worked closely with the author of Advene, who developed project-specific extensions such as the import of OWL ontologies and the export of RDF data, so that film scholars can create semantic video annotations without having to deal with the technical challenges.

[![Image Technical Project Setup](project_setup.png "Technical Project Setup")](project_setup.png)

In order to create a standardized annotation vocabulary, we have created spreadsheet forms with which film scientists can provide domain-specific concepts, terms and descriptions in a familiar software environment. We have developed an automated process to generate the project ontology and the semantic metadata of the video corpus directly from the input data using the RDF mapping language (RML) and the [RML tools](https://rml.io/). The ontology is imported into Advene and makes the domain-specific vocabulary with unique URIs available as annotation tracks in a timeline view so that semantic annotations conforming to the ontology can be exported. Annotations, metadata and the ontology are published via the project's triple store.

