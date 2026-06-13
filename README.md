# DeepFake Detection – Comparação de Modelos de ML

[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.20-orange.svg)](https://www.tensorflow.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-red.svg)](https://pytorch.org/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

## Visão Geral

Este projeto implementa e compara diferentes abordagens de aprendizado de máquina para detecção de **deepfakes** – imagens geradas artificialmente que podem ser usadas para desinformação. O objetivo é classificar imagens faciais como **reais** ou **falsas** (deepfake).

### Modelos implementados

1. **CNN treinada do zero** – Rede neural convolucional simples treinada sobre as imagens redimensionadas para 64×64.
2. **ResNet50 (pré‑treinada) + Classificadores** – Extração de features com a ResNet50 (224×224) e classificação com:
   - Random Forest
   - XGBoost
   - MLP (Multilayer Perceptron)

## Datasets

| Dataset | Imagens | Estrutura |
|---------|---------|------------|
| [Deepfake and Real Images](https://www.kaggle.com/datasets/manjilkarki/deepfake-and-real-images) | ~140k | Pastas `real/` e `fake/` |
| [Deepfake vs Real 60k](https://www.kaggle.com/datasets/prithivsakthiur/deepfake-vs-real-60k) | ~60k | Pastas `Real/` e `Fake/` |

## Metodologia (CRISP‑DM)

O projeto segue as etapas do **CRISP‑DM** (Cross‑Industry Standard Process for Data Mining):

1. **Business Understanding** – Definição do problema e requisitos.
2. **Data Understanding** – Exploração e análise dos datasets.
3. **Data Preparation** – Redimensionamento, normalização, divisão treino/teste.
4. **Modeling** – Treinamento e ajuste dos quatro modelos.
5. **Evaluation** – Comparação usando múltiplas métricas e visualizações.
6. **Deployment** – Salvamento dos modelos para uso futuro.

## Licença

Este projeto está licenciado sob a licença MIT – veja o arquivo [LICENSE](LICENSE) para detalhes.

## Agradecimentos

- Kaggle pelos datasets públicos.
- NVIDIA pelo modelo ResNet50 pré‑treinado.
- Comunidade de código aberto pelas bibliotecas utilizadas.

## Contato

Para dúvidas ou sugestões, abra uma **issue** no GitHub ou entre em contato pelo e‑mail: jonatasfernandes@alu.ufc.br