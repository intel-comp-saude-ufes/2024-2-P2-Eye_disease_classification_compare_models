<div align="center">
<h1> Classificação de doenças oculares: Uma comparação de modelos CNN </h1>

<!-- <--!span><font size="5", > Efficient and Robust 2D-to-BEV Representation Learning via Geometry-guided Kernel Transformer
</font></span> -->

Alefe Gadioli - alefe.gadioli@edu.ufes.br

Priscilla Benevides - priscilla.benevides@edu.ufes.br
<!-- <a href="https://scholar.google.com/citations?user=pCY-bikAAAAJ&hl=zh-CN">Jinwei Yuan</a> -->
<div><a href="https://github.com/intel-comp-saude-ufes/2024-2-P2-Eye_disease_classification_compare_models/blob/main/Projeto_2_Eye_disease_classification_compare_models_v1_pdf.pdf"> Artigo </a> </div> 

<div><a href="https://youtu.be/u0VNPSf90hY"> Video de Apresentação </a> </div> 

</div>

## Descrição do Projeto

A classificação de doenças oculares é uma área de pesquisa dedicada ao desenvolvimento de algoritmos e modelos para identificar com precisão diferentes tipos de doenças oculares a partir de dados de imagem médica. Ela desempenha um papel fundamental ao auxiliar oftalmologistas e profissionais de saúde no diagnóstico e tratamento eficazes das doenças oculares.

A conscientização sobre a saúde ocular, considerando que muitas doenças, como o glaucoma, são assintomáticas nos estágios iniciais é importante para garantir um tratamento adequado e até a cura. O glaucoma pode danificar o nervo óptico e levar à cegueira se não tratado \cite{iapb2020}. Mundialmente, 2,2 bilhões de pessoas têm deficiência visual ou cegueira. No Brasil, são mais de 1,5 milhões, com 74,8\% dos casos sendo evitáveis com diagnóstico precoce.

Este estudo propõe classificar imagens oculares usando aprendizado profundo com os modelos ResNet-18, EfficientNet-B0 e MobileNetV2 no conjunto de dados RFMID, visando diagnósticos iniciais de baixo custo. Os modelos foram escolhidos para integração em sistemas simples e de baixo custo, como triagem e suporte ao diagnóstico. Exemplos de caso de usos: Triagem e Detecção Precoce, Suporte ao Diagnóstico, Planejamento e Monitoramento do Tratamento.

## Resultados

Os resultados obtidos neste estudo mostram que a classificação de doenças oculares utilizando modelos de aprendizado profundo, especificamente ResNet-18, EfficientNet-B0 e MobileNetV2, é viável e apresenta um bom desempenho, considerando para um diagnóstico inicial.

- O modelo ResNet-18 destacou-se com uma acurácia geral de 0,93, especialmente na identificação de retinopatia diabética, com uma precisão e recall de 0,99, e catarata, com uma precisão de 0,97. No entanto, apresentou algumas variações na distinção entre glaucoma e olhos normais, sugerindo possíveis melhorias com maior ajuste e dados adicionais.

- O modelo EfficientNet-B0 obteve uma acurácia de 0,88, mostrando eficiência computacional e uso equilibrado de memória. A presentou uma boa performance na identificação de retinopatia diabética (precisão de 0,91) e catarata (precisão de 0,92), mas com desempenho moderado em glaucoma e olhos normais.

- O modelo MobileNetV2 alcançou uma acurácia de 0,92, destacando-se também na detecção de retinopatia diabética (precisão de 0,98) e catarata (precisão de 0,96), mostrando bom equilíbrio entre precisão e recall para todas as classes. Este modelo é vantajoso para aplicações em dispositivos móveis devido ao menor número de parâmetros e eficiência computacional.

### Escolha do Melhor Modelo

Com base nos resultados apresentados e no problema apresentado, o MobileNetV2 é considerado o melhor modelo para esta aplicação específica de classificação de doenças oculares.

## Requisitos

- **Python 3.x**
- **Bibliotecas:** pandas, numpy, matplotlib, seaborn, tqdm, opencv-python, torch, torchsummary, torchmetrics

## Como Executar

### 1. **Clone o repositório:**
    ```bash
    git clone https://github.com/intel-comp-saude-ufes/2024-2-P2-Eye_disease_classification_compare_models.git
    cd 2024-2-P2-Eye_disease_classification_compare_models

### 2. **Abra o Notebook:**

#### 2.1 **Modelo EfficientNet_B0**
    ```bash
    Abra o notebook: N2_EfficientNet_B0.ipynb
    
#### 2.2 **Modelo ResNet_18**
    ```bash
    Abra o notebook: N2_ResNet_18.ipynb
    
#### 2.3 **Modelo MobileNetV2**
    ```bash
    Abra o notebook: N2_MobileNetV2.ipynb
  
### 3. **Execute o Notebook **

## Referências

- Gulshan, V., Peng, L., Coram, M., Stumpe, M. C., Wu, D., Narayanaswamy, A., ... & Webster, D. R. (2016). Development and validation of a deep learning algorithm for detection of diabetic retinopathy in retinal fundus photographs. JAMA, 316(22), 2402-2410. <div><a href="https://jamanetwork.com/journals/jama/fullarticle/2588763"> Link </a> </div> 
- Ting, D. S., Cheung, C. Y., Lim, G., Tan, G. S., Quang, N. D., Gan, A., ... & Wong, T. Y. (2017). Development and validation of a deep learning system for diabetic retinopathy and related eye diseases using retinal images from multi-ethnic populations with diabetes. JAMA, 318(22), 2211-2223. <div><a href=https://jamanetwork.com/journals/jama/fullarticle/2665775> Link </a> </div> 
- Bismi, D. R., & Na'am, F. M. (2023). Classification of Myopia Using VGG16, VGG19, and InceptionV3 Architectures on Fundus Images. International Journal of Electrical and Computer Engineering, 13(1), 22-30. <div><a href=https://medinftech.org/index.php/medinftech/article/view/8> Link </a> </div> 
- RFMID Dataset. Retinal Fundus Multi-Disease Image Dataset (RFMID). <div><a href=https://ieee-dataport.org/open-access/retinal-fundus-multi-disease-image-dataset-rfmid> Link </a> </div> 
