# Segmentação de Estradas com DeepLabV3+ e ResNet-50

**Aluna:** Sara Souza Rodrigues  
**Projeto 19:** Segmentação de regiões navegáveis em imagens de trânsito utilizando o dataset KITTI Road.

## Descrição do Problema e Objetivo
Este projeto aborda a tarefa de segmentação semântica binária para identificar áreas de estradas e pistas navegáveis a partir de imagens frontais de veículos em movimento. O objetivo principal é desenvolver um modelo robusto utilizando a arquitetura DeepLabV3+ capaz de auxiliar sistemas de percepção visual para veículos autônomos.

## Arquitetura e Tecnologias
* **Modelo:** DeepLabV3+ (com Atrous Spatial Pyramid Pooling - ASPP)
* **Backbone:** ResNet-50 (pesos pré-treinados no ImageNet)
* **Framework:** PyTorch & Segmentation Models PyTorch (SMP)
* **Função de Perda:** Dice Loss

## Experimentos Realizados
Para cumprir a investigação experimental obrigatória, avaliou-se o impacto da resolução das imagens de entrada no desempenho do modelo:
1. **Experimento 1:** Imagens redimensionadas para 256x256 pixels.
2. **Experimento 2:** Imagens redimensionadas para 512x512 pixels.

## Principais Resultados Obtidos
*(Substitua os valores abaixo pelos números que apareceram na tabela do seu Passo 7)*

| Métrica | Exp 1 (256x256) | Exp 2 (512x512) |
| :--- | :---: | :---: |
| **IoU** | 0.XXXX | 0.XXXX |
| **Precisão** | 0.XXXX | 0.XXXX |
| **Recall** | 0.XXXX | 0.XXXX |
| **F1-Score** | 0.XXXX | 0.XXXX |

## Instruções para Execução
1. Abra o arquivo `projeto19_segmentacao.ipynb` no ambiente do Google Colab.
2. Ative o acelerador de Hardware para **T4 GPU** em Ambiente de Execução.
3. Execute todas as células sequencialmente. O download e extração do dataset KITTI ocorrerão automaticamente na máquina virtual.

## Referências e Links
* Link para o Artigo Científico (PDF): [Clique aqui para ler](./artigo_sbc.pdf)
* Dataset KITTI Road: http://www.cvlibs.net/datasets/kitti/eval_road.php
