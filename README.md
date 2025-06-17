# Awesome Chart Understanding

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![PRWelcome](https://img.shields.io/badge/PRs-Welcome-red)](https://img.shields.io/badge/PRs-Welcome-red)
[![arXiv](https://img.shields.io/badge/arXiv-2403.12027-b31b1b.svg?style=flat)](https://arxiv.org/abs/2403.12027)

**🔥🔥 Our survey paper has been accepted by IEEE TKDE! 🔥🔥**

A curated list of recent and past chart understanding work based on our IEEE TKDE survey paper: [From Pixels to Insights: A Survey on Automatic Chart Understanding in the Era of Large Foundation Models](https://arxiv.org/abs/2403.12027).

**The repository will be continuously updated 📝. Don't forget to hit the ⭐️ and stay tuned!**

**If you find this resource beneficial for your research, please do not hesitate to cite the paper referenced in the [Citation](#citation) section. Thank you!**


## Table of Contents
*  [Tasks and Datasets](#tasks-and-datasets)
	*  [Chart Question Answering](#chart-question-answering)
	*  [Chart Captioning (Summarization)](#chart-captioning-summarization)
	*  [Factual Inconsistency Detection for Chart Captioning](#factual-inconsistency-detection-for-chart-captioning)
	*  [Chart Fact-checking](#chart-fact-checking)
	*  [Chart Caption Factual Error Correction](#chart-caption-factual-error-correction)
 	*  [Chart to Code](#chart-to-code)
*  [Methods](#methods)
	*  [Classification-based Methods](#classification-based-methods)
	*  [Generation-based Methods](#generation-based-methods)
 	*  [Tool Augmentation](#tool-augmentation)
*  [Evaluation](#evaluation)
*  [Analysis](#analysis)
*  [Citation](#citation)

## Tasks and Datasets

### Chart Question Answering

**Factoid Questions**

- __DVQA: Understanding Data Visualizations via Question Answering.__ 

  _Kushal Kafle, Brian Price, Scott Cohen, Christopher Kanan._ <img src='https://img.shields.io/badge/CVPR-2018-yellow'> <a href='https://openaccess.thecvf.com/content_cvpr_2018/papers/Kafle_DVQA_Understanding_Data_CVPR_2018_paper.pdf'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/kushalkafle/DVQA_dataset'><img src='https://img.shields.io/badge/Dataset-red'></a>

- __FigureQA: An Annotated Figure Dataset for Visual Reasoning.__ 

  _Samira Ebrahimi Kahou, Vincent Michalski, Adam Atkinson, Akos Kadar, Adam Trischler, Yoshua Bengio._ <img src='https://img.shields.io/badge/ICLR_Workshop-2018-yellow'> <a href='https://arxiv.org/abs/1710.07300'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://www.microsoft.com/en-us/research/project/figureqa-dataset/'><img src='https://img.shields.io/badge/Dataset-red'></a>

- __LEAF-QA: Locate, Encode & Attend for Figure Question Answering.__ 

  _Ritwick Chaudhry, Sumit Shekhar, Utkarsh Gupta, Pranav Maneriker, Prann Bansal, Ajay Joshi._ <img src='https://img.shields.io/badge/WACV-2020-yellow'> <a href='https://openaccess.thecvf.com/content_WACV_2020/papers/Chaudhry_LEAF-QA_Locate_Encode__Attend_for_Figure_Question_Answering_WACV_2020_paper.pdf'><img src='https://img.shields.io/badge/PDF-blue'></a>

- __STL-CQA: Structure-based Transformers with Localization and Encoding for Chart Question Answering.__ 

  _Hrituraj Singh, Sumit Shekhar._ <img src='https://img.shields.io/badge/EMNLP-2020-yellow'> <a href='https://aclanthology.org/2020.emnlp-main.264/'><img src='https://img.shields.io/badge/PDF-blue'></a>

- __PlotQA: Reasoning over Scientific Plots.__ 

  _Nitesh Methani, Pritha Ganguly, Mitesh M. Khapra, Pratyush Kumar._ <img src='https://img.shields.io/badge/WACV-2020-yellow'> <a href='https://arxiv.org/abs/1909.00997'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/NiteshMethani/PlotQA'><img src='https://img.shields.io/badge/Dataset-red'></a>

- __MapQA: A Dataset for Question Answering on Choropleth Maps.__ 

  _Shuaichen Chang, David Palzer, Jialin Li, Eric Fosler-Lussier, Ningchuan Xiao._ <img src='https://img.shields.io/badge/Arxiv-2022-yellow'> <a href='https://arxiv.org/abs/2211.08545'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/OSU-slatelab/MapQA'><img src='https://img.shields.io/badge/Dataset-red'></a>
  

- __ChartQA: A Benchmark for Question Answering about Charts with Visual and Logical Reasoning.__ 

  _Ahmed Masry, Xuan Long Do, Jia Qing Tan, Shafiq Joty, Enamul Hoque._ <img src='https://img.shields.io/badge/ACL_Findings-2022-yellow'> <a href='https://aclanthology.org/2022.findings-acl.177/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/vis-nlp/ChartQA'><img src='https://img.shields.io/badge/Dataset-red'></a>
  

- __SciGraphQA: A Large-Scale Synthetic Multi-Turn Question-Answering Dataset for Scientific Graphs.__

  _Shengzhi Li, Nima Tajbakhsh._ <img src='https://img.shields.io/badge/Arxiv-2023-yellow'> <a href='https://arxiv.org/abs/2308.03349'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/findalexli/SciGraphQA'><img src='https://img.shields.io/badge/Dataset-red'></a>
  


- __MMC: Advancing Multimodal Chart Understanding with Large-scale Instruction Tuning.__ 

  _Fuxiao Liu, Xiaoyang Wang, Wenlin Yao, Jianshu Chen, Kaiqiang Song, Sangwoo Cho, Yaser Yacoob, Dong Yu._ <img src='https://img.shields.io/badge/NAACL-2024-yellow'> <a href='https://arxiv.org/abs/2311.10774'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/FuxiaoLiu/MMC'><img src='https://img.shields.io/badge/Dataset-red'></a>
  

- __MathVista: Evaluating Math Reasoning in Visual Contexts with GPT-4V, Bard, and Other Large Multimodal Models.__ 

  _Pan Lu, Hritik Bansal, Tony Xia, Jiacheng Liu, Chunyuan Li, Hannaneh Hajishirzi, Hao Cheng, Kai-Wei Chang, Michel Galley, Jianfeng Gao._ <img src='https://img.shields.io/badge/ICLR-2024-yellow'> <a href='https://arxiv.org/abs/2310.02255'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/datasets/AI4Math/MathVista'><img src='https://img.shields.io/badge/Dataset-red'></a>


- __ChartBench: A Benchmark for Complex Visual Reasoning in Charts.__ 

  _Zhengzhuo Xu, Sinan Du, Yiyan Qi, Chengjin Xu, Chun Yuan, Jian Guo._ <img src='https://img.shields.io/badge/Arxiv-2023-yellow'> <a href='https://arxiv.org/abs/2312.15915'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/datasets/SincereX/ChartBench'><img src='https://img.shields.io/badge/Dataset-red'></a>

- __Multimodal ArXiv: A Dataset for Improving Scientific Comprehension of Large Vision-Language Models.__

  _Lei Li, Yuqi Wang, Runxin Xu, Peiyi Wang, Xiachong Feng, Lingpeng Kong, Qi Liu._ <img src='https://img.shields.io/badge/Arxiv-2024-yellow'> <a href='https://arxiv.org/abs/2403.00231'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/datasets/MMInstruction/ArxivQA'><img src='https://img.shields.io/badge/Dataset-red'></a>
  
- __Evaluating Task-based Effectiveness of MLLMs on Charts.__

  _Yifan Wu, Lutao Yan, Yuyu Luo, Yunhai Wang, Nan Tang._ <img src='https://img.shields.io/badge/Arxiv-2024-yellow'> <a href='https://arxiv.org/abs/2405.07001'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://anonymous.4open.science/r/ChartInsights-D43E'><img src='https://img.shields.io/badge/Dataset-red'></a>

- __CharXiv: Charting Gaps in Realistic Chart Understanding in Multimodal LLMs.__

  _Zirui Wang, Mengzhou Xia, Luxi He, Howard Chen, Yitao Liu, Richard Zhu, Kaiqu Liang, Xindi Wu, Haotian Liu, Sadhika Malladi, Alexis Chevalier, Sanjeev Arora, Danqi Chen._ <img src='https://img.shields.io/badge/Arxiv-2024-yellow'> <a href='https://arxiv.org/pdf/2406.18521'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/datasets/princeton-nlp/CharXiv'><img src='https://img.shields.io/badge/Dataset-red'></a>

- __ChartMoE: Mixture of Expert Connector for Advanced Chart Understanding.__ 

  _Zhengzhuo Xu⁺, Bowen Qu⁺, Yiyan Qi⁺, Sinan Du, Chengjin Xu, Chun Yuan, Jian Guo._ <img src='https://img.shields.io/badge/ICLR-2025-yellow'> <a href='https://arxiv.org/abs/2409.03277'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/IDEA-FinAI/chartmoe'><img src='https://img.shields.io/badge/Model-red'></a>

**Long-form Questions**  

- __OpenCQA: Open-ended Question Answering with Charts.__ 

  _Shankar Kantharaj, Xuan Long Do, Rixie Tiffany Leong, Jia Qing Tan, Enamul Hoque, Shafiq Joty._ <img src='https://img.shields.io/badge/EMNLP-2022-yellow'> <a href='https://aclanthology.org/2022.emnlp-main.811/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/vis-nlp/OpenCQA'><img src='https://img.shields.io/badge/Dataset-red'></a>


### Chart Captioning (Summarization)

- __Neural Data-Driven Captioning of Time-Series Line Charts.__ 

  _Andrea Spreafico, Giuseppe Carenini._ <img src='https://img.shields.io/badge/AVI-2020-yellow'> <a href='https://dl.acm.org/doi/abs/10.1145/3399715.3399829'><img src='https://img.shields.io/badge/PDF-blue'></a> 

- __Figure Captioning with Relation Maps for Reasoning.__ 

  _Charles Chen, Ruiyi Zhang, Eunyee Koh, Sungchul Kim, Scott Cohen, Ryan Rossi._ <img src='https://img.shields.io/badge/WACV-2020-yellow'> <a href='https://openaccess.thecvf.com/content_WACV_2020/papers/Chen_Figure_Captioning_with_Relation_Maps_for_Reasoning_WACV_2020_paper.pdf'><img src='https://img.shields.io/badge/PDF-blue'></a>


- __Chart-to-Text: Generating Natural Language Descriptions for Charts by Adapting the Transformer Model.__ 

  _Jason Obeid, Enamul Hoque._ <img src='https://img.shields.io/badge/INLG-2020-yellow'> <a href='https://aclanthology.org/2020.inlg-1.20/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/JasonObeid/Chart2Text'><img src='https://img.shields.io/badge/Dataset-red'></a>

- __What Will You Tell Me About the Chart? – Automated Description of Charts.__

  _Karolina Seweryn, Katarzyna Lorenc, Anna Wróblewska, Sylwia Sysko-Romańczuk._ <img src='https://img.shields.io/badge/ICONIP-2021-yellow'> <a href='https://link.springer.com/chapter/10.1007/978-3-030-92307-5_2'><img src='https://img.shields.io/badge/PDF-blue'></a>

- __SciCap: Generating Captions for Scientific Figures.__ 

  _Ting-Yao Hsu, C Lee Giles, Ting-Hao Huang._ <img src='https://img.shields.io/badge/EMNLP-2021-yellow'> <a href='https://aclanthology.org/2021.findings-emnlp.277/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/tingyaohsu/SciCap'><img src='https://img.shields.io/badge/Dataset-red'></a>

- __Chart-to-Text: A Large-Scale Benchmark for Chart Summarization.__ 

  _Shankar Kantharaj, Rixie Tiffany Leong, Xiang Lin, Ahmed Masry, Megh Thakkar, Enamul Hoque, Shafiq Joty._ <img src='https://img.shields.io/badge/ACL-2022-yellow'> <a href='https://aclanthology.org/2022.acl-long.277/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/vis-nlp/Chart-to-text'><img src='https://img.shields.io/badge/Dataset-red'></a>
  

- __LineCap: Line Charts for Data Visualization Captioning Models.__ 

  _Anita Mahinpei, Zona Kostic, Chris Tanner._ <img src='https://img.shields.io/badge/IEEE_VIS-2022-yellow'> <a href='https://ieeexplore.ieee.org/abstract/document/9973197'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/anita76/LineCapDataset'><img src='https://img.shields.io/badge/Dataset-red'></a>
  
- __ChartSumm: A Comprehensive Benchmark for Automatic Chart Summarization of Long and Short Summaries.__

  _Raian Rahman, Rizvi Hasan, Abdullah Al Farhad, Md Tahmid Rahman Laskar, Md. Hamjajul Ashmafee, Abu Raihan Mostofa Kamal._ <img src='https://img.shields.io/badge/Canadian_AI-2023-yellow'> <a href='https://arxiv.org/abs/2304.13620'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/pranonrahman/ChartSumm'><img src='https://img.shields.io/badge/Dataset-red'></a>

- __VisText: A Benchmark for Semantically Rich Chart Captioning.__ 

  _Benny Tang, Angie Boggust, Arvind Satyanarayan._ <img src='https://img.shields.io/badge/ACL-2023-yellow'> <a href='https://aclanthology.org/2023.acl-long.401/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/mitvis/vistext'><img src='https://img.shields.io/badge/Dataset-red'></a>

- __FigCaps-HF: A Figure-to-Caption Generative Framework and Benchmark with Human Feedback.__

  _Ashish Singh, Prateek Agarwal, Zixuan Huang, Arpita Singh, Tong Yu, Sungchul Kim, Victor Bursztyn, Nikos Vlassis, Ryan A. Rossi._ <img src='https://img.shields.io/badge/Arxiv-2023-yellow'> <a href='https://arxiv.org/abs/2307.10867'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://figcapshf.github.io/'><img src='https://img.shields.io/badge/Dataset-red'></a>
  

- __Multimodal ArXiv: A Dataset for Improving Scientific Comprehension of Large Vision-Language Models.__

  _Lei Li, Yuqi Wang, Runxin Xu, Peiyi Wang, Xiachong Feng, Lingpeng Kong, Qi Liu._ <img src='https://img.shields.io/badge/Arxiv-2024-yellow'> <a href='https://arxiv.org/abs/2403.00231'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/datasets/MMInstruction/ArxivCap'><img src='https://img.shields.io/badge/Dataset-red'></a>
  

### Factual Inconsistency Detection for Chart Captioning

- __Do LVLMs Understand Charts? Analyzing and Correcting Factual Errors in Chart Captioning.__ 

  _Kung-Hsiang Huang, Mingyang Zhou, Hou Pong Chan, Yi R. Fung, Zhenhailong Wang, Lingyu Zhang, Shih-Fu Chang, Heng Ji._ <img src='https://img.shields.io/badge/ACL_Findings-2024-yellow'> <a href='https://arxiv.org/abs/2312.10160'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/datasets/khhuang/CHOCOLATE'><img src='https://img.shields.io/badge/Dataset-red'></a>


### Chart Fact-checking

- __Reading and Reasoning over Chart Images for Evidence-based Automated Fact-Checking.__ 

  _Mubasharar Akhtar, Oana Cocarascu, Elena Simperl._ <img src='https://img.shields.io/badge/EACL_Findings-2023-yellow'> <a href='https://aclanthology.org/2023.findings-eacl.30/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/mubasharaak/ChartFC_chartBERT'><img src='https://img.shields.io/badge/Dataset-red'></a>

- __ChartCheck: An Evidence-Based Fact-Checking Dataset over Real-World Chart Images.__ 

  _Mubashara Akhtar, Nikesh Subedi, Vivek Gupta, Sahar Tahmasebi, Oana Cocarascu, Elena Simperl._ <img src='https://img.shields.io/badge/Arxiv-2023-yellow'> <a href='https://arxiv.org/abs/2311.07453'><img src='https://img.shields.io/badge/PDF-blue'></a>


### Chart Caption Factual Error Correction

- __Do LVLMs Understand Charts? Analyzing and Correcting Factual Errors in Chart Captioning.__ 

  _Kung-Hsiang Huang, Mingyang Zhou, Hou Pong Chan, Yi R. Fung, Zhenhailong Wang, Lingyu Zhang, Shih-Fu Chang, Heng Ji._ <img src='https://img.shields.io/badge/ACL_Findings-2024-yellow'> <a href='https://arxiv.org/abs/2312.10160'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/datasets/khhuang/CHOCOLATE'><img src='https://img.shields.io/badge/Dataset-red'></a>

### Chart to Code

- __ChartMimic: Evaluating LMM's Cross-Modal Reasoning Capability via Chart-to-Code Generation.__

  _Chufan Shi, Cheng Yang, Yaxin Liu, Bo Shui, Junjie Wang, Mohan Jing, Linran Xu, Xinyu Zhu, Siheng Li, Yuxiang Zhang, Gongye Liu, Xiaomei Nie, Deng Cai, Yujiu Yang_
  <img src='https://img.shields.io/badge/Arxiv-2024-yellow'> <a href='https://arxiv.org/abs/2406.09961'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/ChartMimic/ChartMimic'><img src='https://img.shields.io/badge/Dataset-red'></a>


- __Text2Chart31: Instruction Tuning for Chart Generation with Automatic Feedback.__ <img src='https://img.shields.io/badge/EMNLP Oral-2024-yellow'> <a href='https://arxiv.org/abs/2410.04064'><img src='https://img.shields.io/badge/PDF-blue'></a> <a href='https://github.com/fatemehpesaran310/Text2Chart31'><img src='https://img.shields.io/badge/Dataset-red'></a>

  _Fatemeh Pesaran Zadeh, Juyeon Kim, Jin-Hwa Kim, Gunhee Kim._

- __ChartMoE: Mixture of Expert Connector for Advanced Chart Understanding.__ 

  _Zhengzhuo Xu⁺, Bowen Qu⁺, Yiyan Qi⁺, Sinan Du, Chengjin Xu, Chun Yuan, Jian Guo._ <img src='https://img.shields.io/badge/ICLR-2025-yellow'> <a href='https://arxiv.org/abs/2409.03277'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/IDEA-FinAI/chartmoe'><img src='https://img.shields.io/badge/Model-red'></a>


## Methods

### Classification-based Methods


#### Fixed Output Vocab



- __A Simple Neural Network Module for Relational Reasoning.__ 

  _Adam Santoro, David Raposo, David G.T. Barrett, Mateusz Malinowski, Razvan Pascanu, Peter Battaglia, Timothy Lillicrap._ <img src='https://img.shields.io/badge/NeurIPS-2017-yellow'> <a href='https://papers.nips.cc/paper_files/paper/2017/hash/e6acf4b0f69f6f6e60e9a815938aa1ff-Abstract.html'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/kimhc6028/relational-networks'><img src='https://img.shields.io/badge/Model-green'></a>
  

- __DVQA: Understanding Data Visualizations via Question Answering.__ 

  _Kushal Kafle, Brian Price, Scott Cohen, Christopher Kanan._ <img src='https://img.shields.io/badge/CVPR-2018-yellow'> <a href='https://openaccess.thecvf.com/content_cvpr_2018/papers/Kafle_DVQA_Understanding_Data_CVPR_2018_paper.pdf'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/kushalkafle/DVQA_dataset'><img src='https://img.shields.io/badge/Model-green'></a>

- __MapQA: A Dataset for Question Answering on Choropleth Maps.__ 

  _Shuaichen Chang, David Palzer, Jialin Li, Eric Fosler-Lussier, Ningchuan Xiao._ <img src='https://img.shields.io/badge/Arxiv-2022-yellow'> <a href='https://arxiv.org/abs/2211.08545'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/OSU-slatelab/MapQA'><img src='https://img.shields.io/badge/Model-green'></a>

#### Dynamic Encoding

- __DVQA: Understanding Data Visualizations via Question Answering.__ 

  _Kushal Kafle, Brian Price, Scott Cohen, Christopher Kanan._ <img src='https://img.shields.io/badge/CVPR-2018-yellow'> <a href='https://openaccess.thecvf.com/content_cvpr_2018/papers/Kafle_DVQA_Understanding_Data_CVPR_2018_paper.pdf'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/kushalkafle/DVQA_dataset'><img src='https://img.shields.io/badge/Model-green'></a>

- __Answering Questions about Data Visualizations using Efficient Bimodal Fusion.__ 

  _Kushal Kafle, Robik Shrestha, Brian Price, Scott Cohen, Christopher Kanan._ <img src='https://img.shields.io/badge/WACV-2020-yellow'> <a href='https://openaccess.thecvf.com/content_WACV_2020/papers/Kafle_Answering_Questions_about_Data_Visualizations_using_Efficient_Bimodal_Fusion_WACV_2020_paper.pdf'><img src='https://img.shields.io/badge/PDF-blue'></a>  
  <a href='https://github.com/kushalkafle/PReFIL'><img src='https://img.shields.io/badge/Model-green'></a>

- __LEAF-QA: Locate, Encode & Attend for Figure Question Answering.__ 

  _Ritwick Chaudhry, Sumit Shekhar, Utkarsh Gupta, Pranav Maneriker, Prann Bansal, Ajay Joshi._ <img src='https://img.shields.io/badge/WACV-2020-yellow'> <a href='https://openaccess.thecvf.com/content_WACV_2020/papers/Chaudhry_LEAF-QA_Locate_Encode__Attend_for_Figure_Question_Answering_WACV_2020_paper.pdf'><img src='https://img.shields.io/badge/PDF-blue'></a>


- __PlotQA: Reasoning over Scientific Plots.__ 

  _Nitesh Methani, Pritha Ganguly, Mitesh M. Khapra, Pratyush Kumar._ <img src='https://img.shields.io/badge/WACV-2020-yellow'> <a href='https://arxiv.org/abs/1909.00997'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/NiteshMethani/PlotQA'><img src='https://img.shields.io/badge/Model-green'></a>

#### Pre-trained

- __TaPas: Weakly Supervised Table Parsing via Pre-training.__ 

  _Jonathan Herzig, Pawel Krzysztof Nowak, Thomas Müller, Francesco Piccinno, Julian Eisenschlos._ <img src='https://img.shields.io/badge/ACL-2020-yellow'> <a href='https://aclanthology.org/2020.acl-main.398/'><img src='https://img.shields.io/badge/PDF-blue'></a>  
  <a href='https://github.com/google-research/tapas'><img src='https://img.shields.io/badge/Model-green'></a>

- __STL-CQA: Structure-based Transformers with Localization and Encoding for Chart Question Answering.__ 

  _Hrituraj Singh, Sumit Shekhar._ <img src='https://img.shields.io/badge/EMNLP-2020-yellow'> <a href='https://aclanthology.org/2020.emnlp-main.264/'><img src='https://img.shields.io/badge/PDF-blue'></a>

- __ChartQA: A Benchmark for Question Answering about Charts with Visual and Logical Reasoning.__ 

  _Ahmed Masry, Xuan Long Do, Jia Qing Tan, Shafiq Joty, Enamul Hoque._ <img src='https://img.shields.io/badge/ACL_Findings-2022-yellow'> <a href='https://aclanthology.org/2022.findings-acl.177/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/vis-nlp/ChartQA'><img src='https://img.shields.io/badge/Model-green'></a>

### Generation-based Methods

#### Without Pre-training

- __SciCap: Generating Captions for Scientific Figures.__ 

  _Ting-Yao Hsu, C Lee Giles, Ting-Hao Huang._ <img src='https://img.shields.io/badge/EMNLP-2021-yellow'> <a href='https://aclanthology.org/2021.findings-emnlp.277/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/tingyaohsu/SciCap'><img src='https://img.shields.io/badge/Model-green'></a>

- __Figure Captioning with Relation Maps for Reasoning.__ 

  _Charles Chen, Ruiyi Zhang, Eunyee Koh, Sungchul Kim, Scott Cohen, Ryan Rossi._ <img src='https://img.shields.io/badge/WACV-2020-yellow'> <a href='https://openaccess.thecvf.com/content_WACV_2020/papers/Chen_Figure_Captioning_with_Relation_Maps_for_Reasoning_WACV_2020_paper.pdf'><img src='https://img.shields.io/badge/PDF-blue'></a>

- __Chart-to-Text: Generating Natural Language Descriptions for Charts by Adapting the Transformer Model.__ 

  _Jason Obeid, Enamul Hoque._ <img src='https://img.shields.io/badge/INLG-2020-yellow'> <a href='https://aclanthology.org/2020.inlg-1.20/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/JasonObeid/Chart2Text'><img src='https://img.shields.io/badge/Model-green'></a>

- __Tackling Hallucinations in Neural Chart Summarization.__ 

 _Saad Obaid ul Islam, Iza Škrjanec, Ondřej Dušek, Vera Demberg_ <img src='https://img.shields.io/badge/INLG-2023-yellow'> <a href='https://aclanthology.org/2023.inlg-main.30/'><img src='https://img.shields.io/badge/PDF-blue'></a> <a href='[https://github.com/JasonObeid/Chart2Text](https://github.com/WorldHellow/Hallucinations-C2T)'><img src='https://img.shields.io/badge/Model-green'></a>
 
#### Pre-trained


- __Enhanced Chart Understanding via Visual Language Pre-training on Plot Table Pairs.__ 

  _Mingyang Zhou, Yi Fung, Long Chen, Christopher Thomas, Heng Ji, Shih-Fu Chang._ <img src='https://img.shields.io/badge/ACL_Findings-2023-yellow'> <a href='https://aclanthology.org/2023.findings-acl.85/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/zmykevin/ACL2023_ChartT5'><img src='https://img.shields.io/badge/Model-green'></a>

- __MatCha: Enhancing Visual Language Pretraining with Math Reasoning and Chart Derendering.__

  _Fangyu Liu, Francesco Piccinno, Syrine Krichene, Chenxi Pang, Kenton Lee, Mandar Joshi, Yasemin Altun, Nigel Collier, Julian Eisenschlos._ <img src='https://img.shields.io/badge/ACL-2023-yellow'> <a href='https://aclanthology.org/2023.acl-long.714/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='google/matcha-base'><img src='https://img.shields.io/badge/Model-green'></a>
  
- __UniChart: A Universal Vision-language Pretrained Model for Chart Comprehension and Reasoning.__

  _Ahmed Masry, Parsa Kavehzadeh, Xuan Long Do, Enamul Hoque, Shafiq Joty._ <img src='https://img.shields.io/badge/EMNLP-2023-yellow'> <a href='https://aclanthology.org/2023.emnlp-main.906/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/vis-nlp/UniChart'><img src='https://img.shields.io/badge/Model-green'></a>

- __Pix2Struct: Screenshot Parsing as Pretraining for Visual Language Understanding.__

  _Kenton Lee, Mandar Joshi, Iulia Raluca Turc, Hexiang Hu, Fangyu Liu, Julian Martin Eisenschlos, Urvashi Khandelwal, Peter Shaw, Ming-Wei Chang, Kristina Toutanova._ <img src='https://img.shields.io/badge/ICML-2023-yellow'> <a href='https://proceedings.mlr.press/v202/lee23g/lee23g.pdf'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/google/pix2struct-base'><img src='https://img.shields.io/badge/Model-green'></a>

- __Synthesize Step-by-Step: Tools, Templates and LLMs as Data Generators for Reasoning-Based Chart VQA.__

  _Zhuowan Li, Bhavan Jasani, Peng Tang, Shabnam Ghadar._ <img src='https://img.shields.io/badge/CVPR-2024-yellow'> <a href='https://arxiv.org/abs/2403.16385'><img src='https://img.shields.io/badge/PDF-blue'></a>
  


  
  
### Tool Augmentation
- __DePlot: One-shot visual language reasoning by plot-to-table translation.__

  _Fangyu Liu, Julian Eisenschlos, Francesco Piccinno, Syrine Krichene, Chenxi Pang, Kenton Lee, Mandar Joshi, Wenhu Chen, Nigel Collier, Yasemin Altun._ <img src='https://img.shields.io/badge/ACL_Findings-2023-yellow'> <a href='https://aclanthology.org/2023.findings-acl.660/'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/google/deplot'><img src='https://img.shields.io/badge/Model-green'></a>

  
- __Do LVLMs Understand Charts? Analyzing and Correcting Factual Errors in Chart Captioning.__

  _Kung-Hsiang Huang, Mingyang Zhou, Hou Pong Chan, Yi R. Fung, Zhenhailong Wang, Lingyu Zhang, Shih-Fu Chang, Heng Ji._ <img src='https://img.shields.io/badge/ACL_Findings-2024-yellow'> <a href='https://arxiv.org/abs/2312.10160'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/khhuang/chart-to-table'><img src='https://img.shields.io/badge/Model-green'></a>

- __Do LLMs Work on Charts? Designing Few-Shot Prompts for Chart Question Answering and Summarization.__

  _Xuan Long Do, Mohammad Hassanpour, Ahmed Masry, Parsa Kavehzadeh, Enamul Hoque, Shafiq Joty._ <img src='https://img.shields.io/badge/Arxiv-2023-yellow'> <a href='https://arxiv.org/abs/2312.10610'><img src='https://img.shields.io/badge/PDF-blue'></a>

- __DOMINO: A Dual-System for Multi-step Visual Language Reasoning.__

  _Peifeng Wang, Olga Golovneva, Armen Aghajanyan, Xiang Ren, Muhao Chen, Asli Celikyilmaz, Maryam Fazel-Zarandi._ <img src='https://img.shields.io/badge/Arxiv-2023-yellow'> <a href='https://arxiv.org/abs/2310.02804'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/facebookresearch/dual-system-for-visual-language-reasoning'><img src='https://img.shields.io/badge/Model-green'></a>
  

- __StructChart: Perception, Structuring, Reasoning for Visual Chart Understanding.__

  _Renqiu Xia, Bo Zhang, Haoyang Peng, Hancheng Ye, Xiangchao Yan, Peng Ye, Botian Shi, Yu Qiao, Junchi Yan._ <img src='https://img.shields.io/badge/Arxiv-2023-yellow'> <a href='https://arxiv.org/abs/2309.11268'><img src='https://img.shields.io/badge/PDF-blue'></a>


- __SIMPLOT: Enhancing Chart Question Answering by Distilling Essentials.__

  _Wonjoong Kim, Sangwu Park, Yeonjun In, Seokwon Han, Chanyoung Park._ <img src='https://img.shields.io/badge/Arxiv-2024-yellow'> <a href='https://arxiv.org/abs/2405.00021'><img src='https://img.shields.io/badge/PDF-blue'></a>

- __OneChart: Purify the Chart Structural Extraction via One Auxiliary Token
.__

  _Jinyue Chen, Lingyu Kong, Haoran Wei, Chenglong Liu, Zheng Ge, Liang Zhao, Jianjian Sun, Chunrui Han, Xiangyu Zhang._ <img src='https://img.shields.io/badge/ACM_MM-2024-yellow'> <a href='https://arxiv.org/abs/2404.09987'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/kppkkp/OneChart/tree/main'><img src='https://img.shields.io/badge/Model-green'></a>
  <a href='https://drive.google.com/drive/folders/1YmOvxq0DfOA9YKoyCZDjpnTIkPNoyegQ?usp=sharing'><img src='https://img.shields.io/badge/Dataset-red'></a>

### Large Vision-language Models

**Tailored for Chart Understanding** 


- __ChartLlama: A Multimodal LLM for Chart Understanding and Generation.__ 

  _Yucheng Han, Chi Zhang, Xin Chen, Xu Yang, Zhibin Wang, Gang Yu, Bin Fu, Hanwang Zhang._ <img src='https://img.shields.io/badge/Arxiv-2023-yellow'> <a href='https://arxiv.org/abs/2311.16483'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/tingxueronghua/ChartLlama-code'><img src='https://img.shields.io/badge/Model-green'></a>
  
- __MMC: Advancing Multimodal Chart Understanding with Large-scale Instruction Tuning.__ 

  _Fuxiao Liu, Xiaoyang Wang, Wenlin Yao, Jianshu Chen, Kaiqiang Song, Sangwoo Cho, Yaser Yacoob, Dong Yu._ <img src='https://img.shields.io/badge/NAACL-2024-yellow'> <a href='https://arxiv.org/abs/2311.10774'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/FuxiaoLiu/MMC'><img src='https://img.shields.io/badge/Model-green'></a>
  
- __ChartAssistant: A Universal Chart Multimodal Language Model via Chart-to-Table Pre-training and Multitask Instruction Tuning.__ 

  _Fanqing Meng, Wenqi Shao, Quanfeng Lu, Peng Gao, Kaipeng Zhang, Yu Qiao, Ping Luo._ <img src='https://img.shields.io/badge/ACL Findings-2024-yellow'> <a href='https://arxiv.org/abs/2401.02384'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/OpenGVLab/ChartAst'><img src='https://img.shields.io/badge/Model-green'></a>
  
  
- __ChartInstruct: Instruction Tuning for Chart Comprehension and Reasoning.__ 

  _Ahmed Masry, Mehrad Shahmohammadi, Md Rizwan Parvez, Enamul Hoque, Shafiq Joty._ <img src='https://img.shields.io/badge/ACL Findings-2024-yellow'> <a href='https://arxiv.org/abs/2403.09028'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/vis-nlp/ChartInstruct'><img src='https://img.shields.io/badge/Model-green'></a>
  
  
- __ChartX & ChartVLM: A Versatile Benchmark and Foundation Model for Complicated Chart Reasoning.__ 

  _Renqiu Xia, Bo Zhang, Hancheng Ye, Xiangchao Yan, Qi Liu, Hongbin Zhou, Zijun Chen, Min Dou, Botian Shi, Junchi Yan, Yu Qiao._ <img src='https://img.shields.io/badge/Arxiv-2024-yellow'> <a href='https://arxiv.org/abs/2402.12185'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/UniModal4Reasoning/ChartVLM'><img src='https://img.shields.io/badge/Model-green'></a>

- __FigurA11y: AI Assistance for Writing Scientific Alt Text.__ 

  _Nikhil Singh, Andrew Head, Lucy Lu Wang, Jonathan Bragg._ <img src='https://img.shields.io/badge/Arxiv-2024-yellow'> <a href='https://www.llwang.net/assets/pdf/2024_singh_figura11y_iui.pdf'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/allenai/figura11y'><img src='https://img.shields.io/badge/Model-green'></a>

- __Chart-based Reasoning: Transferring Capabilities from LLMs to VLMs.__ 

  _Victor Carbune, Hassan Mansoor, Fangyu Liu, Rahul Aralikatte, Gilles Baechler, Jindong Chen, Abhanshu Sharma._ <img src='https://img.shields.io/badge/NAACL Findings-2024-yellow'> <a href='https://arxiv.org/abs/2403.12596'><img src='https://img.shields.io/badge/PDF-blue'></a>

- __TinyChart: Efficient Chart Understanding with Visual Token Merging and Program-of-Thoughts Learning.__ 

  _Liang Zhang, Anwen Hu, Haiyang Xu, Ming Yan, Yichen Xu, Qin Jin, Ji Zhang, Fei Huang._ <img src='https://img.shields.io/badge/EMNLP-2024-yellow'> <a href='https://arxiv.org/abs/2404.16635'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/X-PLUG/mPLUG-DocOwl/tree/main/TinyChart'><img src='https://img.shields.io/badge/Model-green'></a>

- __ChartGemma: Visual Instruction-tuning for Chart Reasoning in the Wild.__ 

  _Ahmed Masry, Megh Thakkar, Aayush Bajaj, Aaryaman Kartha, Enamul Hoque, Shafiq Joty._ <img src='https://img.shields.io/badge/COLING Industry-2025-yellow'> <a href='https://arxiv.org/abs/2407.04172v1'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/vis-nlp/ChartGemma'><img src='https://img.shields.io/badge/Model-green'></a>

- __Multimodal Self-Instruct: Synthetic Abstract Image and Visual Reasoning Instruction Using Language Model__
  
  _Wenqi Zhang, Zhenglin Cheng, Yuanyu He, Mengna Wang, Yongliang Shen, Zeqi Tan, Guiyang Hou, Mingqian He, Yanna Ma, Weiming Lu, Yueting Zhuang._ <img src='https://img.shields.io/badge/EMNLP-2024-yellow'> <a href='https://arxiv.org/abs/2407.07053'><img src='https://img.shields.io/badge/PDF-blue'></a>
<a href='https://github.com/zwq2018/Multi-modal-Self-instruct'><img src='https://img.shields.io/badge/Model-green'></a>

- __Distill Visual Chart Reasoning Ability from LLMs to MLLMs__

  _Wei He, Zhiheng Xi, Wanxu Zhao, Xiaoran Fan, Yiwen Ding, Zifei Shan, Tao Gui, Qi Zhang, Xuanjing Huang._ <img src='https://img.shields.io/badge/Arxiv-2024-yellow'> <a href='https://arxiv.org/abs/2410.18798'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/hewei2001/ReachQA'><img src='https://img.shields.io/badge/Model-green'></a>

- __Why Vision Language Models Struggle with Visual Arithmetic? Towards Enhanced Chart and Geometry Understanding__

  _Kung-Hsiang Huang, Can Qin, Haoyi Qiu, Philippe Laban, Shafiq Joty, Caiming Xiong, Chien-Sheng Wu._ <img src='https://img.shields.io/badge/Arxiv-2025-yellow'> <a href='https://arxiv.org/abs/2502.11492'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/datasets/Salesforce/CogAlign'><img src='https://img.shields.io/badge/Dataset-red'></a>
  <a href='https://huggingface.co/Salesforce/cogalign-internvl2_5-mpo-4b'><img src='https://img.shields.io/badge/Model-green'></a>


**General-purpose**

- __Visual Instruction Tuning.__ 

  _Haotian Liu, Chunyuan Li, Qingyang Wu, Yong Jae Lee._ <img src='https://img.shields.io/badge/NeurIPS-2023-yellow'> <a href='https://arxiv.org/abs/2304.08485'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/haotian-liu/LLaVA'><img src='https://img.shields.io/badge/Model-green'></a>

- __mPLUG-Owl: Modularization Empowers Large Language Models with Multimodality.__ 

  _Qinghao Ye, Haiyang Xu, Guohai Xu, Jiabo Ye, Ming Yan, Yiyang Zhou, Junyang Wang, Anwen Hu, Pengcheng Shi, Yaya Shi, Chenliang Li, Yuanhong Xu, Hehong Chen, Junfeng Tian, Qian Qi, Ji Zhang, Fei Huang._ <img src='https://img.shields.io/badge/Arxiv-2023-yellow'> <a href='https://arxiv.org/abs/2304.14178'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/X-PLUG/mPLUG-Owl'><img src='https://img.shields.io/badge/Model-green'></a>

- __mPLUG-Owl2: Revolutionizing Multi-modal Large Language Model with Modality Collaboration.__ 

  _Qinghao Ye, Haiyang Xu, Jiabo Ye, Ming Yan, Anwen Hu, Haowei Liu, Qi Qian, Ji Zhang, Fei Huang, Jingren Zhou._ <img src='https://img.shields.io/badge/CVPR-2024-yellow'> <a href='https://arxiv.org/abs/2311.04257'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/X-PLUG/mPLUG-Owl'><img src='https://img.shields.io/badge/Model-green'></a>

- __mPLUG-DocOwl 1.5: Unified Structure Learning for OCR-free Document Understanding__ 

  _Anwen Hu, Haiyang Xu, Jiabo Ye, Ming Yan, Liang Zhang, Bo Zhang, Chen Li, Ji Zhang, Qin Jin, Fei Huang, Jingren Zhou._ <img src='https://img.shields.io/badge/Arxiv-2024-yellow'> <a href='https://arxiv.org/abs/2403.12895'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/X-PLUG/mPLUG-DocOwl/tree/main/DocOwl1.5'><img src='https://img.shields.io/badge/Model-green'></a>  

- __SPHINX: The Joint Mixing of Weights, Tasks, and Visual Embeddings for Multi-modal Large Language Models.__ 

  _Ziyi Lin, Chris Liu, Renrui Zhang, Peng Gao, Longtian Qiu, Han Xiao, Han Qiu, Chen Lin, Wenqi Shao, Keqin Chen, Jiaming Han, Siyuan Huang, Yichi Zhang, Xuming He, Hongsheng Li, Yu Qiao._ <img src='https://img.shields.io/badge/Arxiv-2023-yellow'> <a href='https://arxiv.org/abs/2311.07575'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://github.com/Alpha-VLLM/LLaMA2-Accessory/tree/main/SPHINX'><img src='https://img.shields.io/badge/Model-green'></a>


- __Gemini: A Family of Highly Capable Multimodal Models.__ 

  _Gemini Team Google._ <img src='https://img.shields.io/badge/Arxiv-2023-yellow'> <a href='https://arxiv.org/abs/2312.11805'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://gemini.google.com/'><img src='https://img.shields.io/badge/Interface-darkgreen'></a>

- __GPT-4V.__ 

  _OpenAI._ <img src='https://img.shields.io/badge/Year-2023-yellow'> <a href='https://openai.com/research/gpt-4v-system-card'><img src='https://img.shields.io/badge/Website-blue'></a>
  <a href='https://chat.openai.com/'><img src='https://img.shields.io/badge/Interface-darkgreen'></a>

- __Introducing the next generation of Claude (Claude 3).__ 

  _Antropic._ <img src='https://img.shields.io/badge/Year-2023-yellow'> <a href='https://www.anthropic.com/news/claude-3-family'><img src='https://img.shields.io/badge/Website-blue'></a>
  <a href='https://claude.ai/'><img src='https://img.shields.io/badge/Interface-darkgreen'></a>  

- __Why Vision Language Models Struggle with Visual Arithmetic? Towards Enhanced Chart and Geometry Understanding__

  _Kung-Hsiang Huang, Can Qin, Haoyi Qiu, Philippe Laban, Shafiq Joty, Caiming Xiong, Chien-Sheng Wu._ <img src='https://img.shields.io/badge/Arxiv-2025-yellow'> <a href='https://arxiv.org/abs/2502.11492'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/datasets/Salesforce/CogAlign'><img src='https://img.shields.io/badge/Dataset-red'></a>
  <a href='https://huggingface.co/Salesforce/cogalign-internvl2_5-mpo-4b'><img src='https://img.shields.io/badge/Model-green'></a>

## Evaluation

### Faithfulness/ Factuality

- __Do LVLMs Understand Charts? Analyzing and Correcting Factual Errors in Chart Captioning.__ 

  _Kung-Hsiang Huang, Mingyang Zhou, Hou Pong Chan, Yi R. Fung, Zhenhailong Wang, Lingyu Zhang, Shih-Fu Chang, Heng Ji._ <img src='https://img.shields.io/badge/ACL_Findings-2024-yellow'> <a href='https://arxiv.org/abs/2312.10160'><img src='https://img.shields.io/badge/PDF-blue'></a>
  <a href='https://huggingface.co/khhuang/chartve'><img src='https://img.shields.io/badge/Model-green'></a>

## Analysis

- __Are Large Vision Language Models up to the Challenge of Chart Comprehension and Reasoning? An Extensive Investigation into the Capabilities and Limitations of LVLMs.__

  _Mohammed Saidul Islam, Raian Rahman, Ahmed Masry, Md Tahmid Rahman Laskar, Mir Tafseer Nayeem, Enamul Hoque._ <img src='https://img.shields.io/badge/Arxiv-2024-yellow'> <a href='https://arxiv.org/abs/2406.00257'><img src='https://img.shields.io/badge/PDF-blue'></a>

- __On the Perception Bottleneck of VLMs for Chart Understanding.__

  _Junteng Liu, Weihao Zeng, Xiwen Zhang, Yijun Wang, Zifei Shan, Junxian He._ <img src='https://img.shields.io/badge/Arxiv-2025-yellow'> <a href='https://arxiv.org/abs/2503.18435'><img src='https://img.shields.io/badge/PDF-blue'></a>
  
## Citation

```bibtex
@article{huang-etal-2024-chart,
    title = "From Pixels to Insights: A Survey on Automatic Chart Understanding in the Era of Large Foundation Models",
    author = "Huang, Kung-Hsiang and Chan, Hou Pong and Fung, Yi R. and Qiu, Haoyi and Zhou, Mingyang and Joty, Shafiq and Chang, Shih-Fu and Ji, Heng",
    year={2024},
    journal={IEEE Transactions on Knowledge and Data Engineering (TKDE)},
}
```
