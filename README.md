# HS_code

The code groups in this repository were used in a meta-analysis study of gene expression data related to heat stress in human and mouse ([1](#1-yonezawa-s-bono-h-meta-analysis-of-heat-stressed-transcriptomes-using-the-public-gene-expression-database-from-human-and-mouse-samples-biorxiv-2023-p-20230430537112-doi10110120230430537112)). Also, this repository is [MIT LICENSE](./LICENSE).

All code is written in Jupyter notebook format for easy reproduction.

All figures written using these codes can be viewed and downloaded from figshare collection file ([2](#2-yonezawa-s-meta-analysis-of-heat-stressed-gene-expresssion-data-in-human-and-mouse-figshare-collection-2023-url-httpsdoiorg106084m9figsharec6564487v2)).

&nbsp;

## [1_bar-graph_dataset](./1_bar-graph_dataset)

### How we used this codes (1)

These scripts were used to visualize metadata of gene expression data collected from public databases(Gene Expression Omnibus).

- [HS_sample.ipynb](./1_bar-graph_dataset/HS_sample.ipynb)

  - Script for visualization of cell types, tissues, and other information in a stacked bar graph.

- [HS_treatment.ipynb](./1_bar-graph_dataset/HS_treatment.ipynb)

  - Script to visualize the exposure time at a certain temperature condition as a bar graph.

- [HS_temperature.ipynb](./1_bar-graph_dataset/HS_temperature.ipynb)

  - Script for visualization of temperature condition information (degree, ℃) in a bar graph.

&nbsp;

## [2_scatter-plot_HNscore](./2_scatter-plot_HNscore)

### How we used this codes (2)

Mainly, we visualized the characteristics of the genes by creating scatter plots with respect to the HN-score (index of analysis: see ([1](#1-yonezawa-s-bono-h-meta-analysis-of-heat-stressed-transcriptomes-using-the-public-gene-expression-database-from-human-and-mouse-samples-biorxiv-2023-p-20230430537112-doi10110120230430537112)) for details). 
__Note that the code in the Hypoxia_code repository (<https://github.com/no85j/hypoxia_code>) was used to calculate the HN-score.__

#### 1. Visualization of HN-score calculated for all genes

- [scatter_plot_HNscore_human.ipynb](./2_scatter-plot_HNscore/scatter_plot_HNscore_human.ipynb)
- [scatter_plot_HNscore_mouse.ipynb](./2_scatter-plot_HNscore/scatter_plot_HNscore_mouse.ipynb)

#### 2. Visualization of the distribution of HN-scores of genes shared by human and mouse

- [scatter_plot_HNscore_human_vs_mouse.ipynb](./2_scatter-plot_HNscore/scatter_plot_HNscore_human_vs_mouse.ipynb)

#### 3. Visualization integrating HN-score and ChiP-seq data

- [scatter_plot_HNscore_ChIP-seq_HSF1.ipynb](./2_scatter-plot_HNscore/scatter_plot_HNscore_ChIP-seq_HSF1.ipynb)
- [scatter_plot_HNscore_ChIP-seq_HSF2.ipynb](./2_scatter-plot_HNscore/scatter_plot_HNscore_ChIP-seq_HSF2.ipynb)
- [scatter_plot_HNscore_ChIP-seq_PPARGC1A.ipynb](./2_scatter-plot_HNscore/scatter_plot_HNscore_ChIP-seq_PPARGC1A.ipynb)

#### < Note1 >

ChIP-seq data were obtained using the "Tatget genes" function of the ChIP-Atlas database([3](#3-oki-s-ohta-t-shioi-g-hatanaka-h-ogasawara-o-okuda-y-et-al-chip-atlas-a-data-mining-suite-powered-by-full-integration-of-public-chip-seq-data-embo-rep-201819-doi1015252embr201846255)).

## [3_stacked_bar_graph](./3_stacked_bar_graph)

### How we used this codes (3)

These codes were visualized in stacked bar graphs to show which HN-score values of common upregulated downregulated genes were derived from what samples, sequencing methods, and experimental conditions.
The figures created by these codes can be accessed from the figshare file as Figure S2 (URL: <https://doi.org/10.6084/m9.figshare.22559752.v4>).

- A_sample_type directory
  - [HNscore_HN5_sample_type_human.ipynb](./3_stacked_bar_graph/A_sample_type/HNscore_HN5_sample_type_human.ipynb)
  - [HNscore_HN5_sample_type_mouse.ipynb](./3_stacked_bar_graph/A_sample_type/HNscore_HN5_sample_type_mouse.ipynb)
  - [stacked_bar_HNscore_sample.ipynb](./3_stacked_bar_graph/A_sample_type/stacked_bar_HNscore_sample.ipynb) (for visualization)

&nbsp;

- B_sequencing_method directory
  - [HNscore_HN5_sequencing_type_human.ipynb](./3_stacked_bar_graph/B_sequencing_method/HNscore_HN5_sequencing_type_human.ipynb)
  - [HNscore_HN5_sequencing_type_mouse.ipynb](./3_stacked_bar_graph/B_sequencing_method/HNscore_HN5_sequencing_type_mouse.ipynb)
  - [stacked_bar_HNscore_sequencing.ipynb](./3_stacked_bar_graph/B_sequencing_method/stacked_bar_HNscore_sequencing.ipynb) (for visualization)

&nbsp;

- C_condition directory
  - [HNscore_HN5_condition_human.ipynb](./3_stacked_bar_graph/C_condition/HNscore_HN5_condition_human.ipynb)
  - [HNscore_HN5_condition_mouse.ipynb](./3_stacked_bar_graph/C_condition/HNscore_HN5_condition_mouse.ipynb)
  - [stacked_bar_HNscore_condition.ipynb](./3_stacked_bar_graph/C_condition/stacked_bar_HNscore_condition.ipynb) (for visualization)

#### < Note2 >

- Utilizing the human and mouse metadata in Table S1 and 2, we are creating a figure.

- Table S1 (URL: <https://doi.org/10.6084/m9.figshare.22565212.v2>)
- Table S2 (URL: <https://doi.org/10.6084/m9.figshare.22565311.v4>)

&nbsp;

&nbsp;

#### References

##### 1. Yonezawa S, Bono H. Meta-analysis of heat-stressed transcriptomes using the public gene expression database from human and mouse samples. bioRxiv. 2023. p. 2023.04.30.537112. doi:10.1101/2023.04.30.537112

##### 2. Yonezawa S. Meta-analysis of Heat-stressed gene expresssion data in human and mouse. figshare. Collection. 2023. URL: <https://doi.org/10.6084/m9.figshare.c.6564487.v2>

##### 3. Oki S, Ohta T, Shioi G, Hatanaka H, Ogasawara O, Okuda Y, et al. ChIP-Atlas: a data-mining suite powered by full integration of public ChIP-seq data. EMBO Rep. 2018;19. doi:10.15252/embr.201846255
