# 🕵️ No Big Deal (Roblox) - Head Detection Model

![Roboflow](https://img.shields.io/badge/Roboflow-Model-purple)
![Model](https://img.shields.io/badge/Model-RF--DETR%20(Nano)-blue)
![Status](https://img.shields.io/badge/Status-Active-success)

Este repositório contém um modelo de Visão Computacional treinado para detectar a classe `cabeca` (cabeça dos jogadores) dentro do jogo **No Big Deal** no Roblox.

O projeto foi desenvolvido e treinado utilizando a plataforma [Roboflow](https://roboflow.com).

## 🎮 Sobre o Jogo
**Nome:** No Big Deal  
**Plataforma:** Roblox  
**Link do Jogo:** [Jogar Agora](https://www.roblox.com/games/18112334178/No-Big-Deal)

## 📊 Desempenho do Modelo (v9)

O modelo "TreinamentoFinal" (v9) apresentou resultados de alta precisão nos testes de validação.

| Métrica | Valor | Descrição |
| :--- | :---: | :--- |
| **mAP@50** | **93.9%** | Precisão Média (Mean Average Precision) |
| **Precision** | **93.4%** | Taxa de acerto nas detecções positivas |
| **Recall** | **92.5%** | Capacidade de encontrar todas as ocorrências |

> **Nota:** O modelo utiliza a arquitetura **RF-DETR (Nano)**, otimizada para inferência rápida.

## 📷 Detalhes do Dataset

*   **Total de Imagens:** 4.136
*   **Classes:** `cabeca`
*   **Distribuição:**
    *   Treino: 70% (2.896 imagens)
    *   Validação: 20% (828 imagens)
    *   Teste: 10% (412 imagens)

### Pré-processamento
As imagens foram submetidas aos seguintes processos antes do treinamento:
1.  **Auto-Orient:** Aplicado.
2.  **Resize:** 640x345 (Stretch/Fill com corte central).
3.  **Grayscale:** Aplicado (O modelo foi treinado em escala de cinza).
