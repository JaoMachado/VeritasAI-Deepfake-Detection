# VeritasAI 🤖

**VeritasAI: UMA PROPOSTA PARA DETECÇÃO DE IMAGENS ARTIFICIAIS**

Um sistema de classificação de imagens baseado em Redes Neurais Convolucionais (CNNs) capaz de distinguir imagens reais de imagens geradas por Inteligência Artificial (Deepfakes).

Este projeto foi desenvolvido por [João Pedro Machado Silva](https://www.linkedin.com/in/jaomachado/) e [Leonardo Solovijovas Santos](https://www.linkedin.com/in/leonardo-solovijovas-santos/),  com orientação do Prof. [Gabriel Marcelino Alves](https://www.linkedin.com/in/alvesmgabriel/), como parte de um trabalho de pesquisa apresentado na **SECITEM**.

---

## 🚀 Principais Resultados

O modelo alcançou uma performance robusta, validando a abordagem para detecção de conteúdo sintético:

* **Acurácia de 95,6%** no conjunto de validação.
* **F1-Score médio de 0,96**
* Implementação de uma **"zona de incerteza"** (para predições entre 0.4 e 0.6) para identificar casos ambíguos que necessitam de revisão humana, aumentando a confiabilidade.

### Matriz de Confusão

A matriz de confusão abaixo ilustra o desempenho do modelo no conjunto de validação:

<img width="1034" height="531" alt="image" src="https://github.com/user-attachments/assets/3dd1f122-c0db-4464-b74d-c64016b4ce37" />

**(Fonte: Os autores)**

---

## 🛠️ Metodologia e Tecnologias

O VeritasAI foi construído utilizando uma arquitetura moderna e eficiente:

* **Modelo:** Rede Neural Convolucional (CNN).
* **Arquitetura Base:** **EfficientNetB0**.
* **Técnicas:** `Transfer Learning`, `Fine-Tuning` e `Data Augmentation` para aumentar a robustez e generalização do modelo.
* **Dataset:** O treinamento foi realizado com o conjunto "AI vs Human-Generated Images" (Kaggle), contendo 70.000 imagens balanceadas.
* **Frameworks (Sugestão):** Python, TensorFlow, Keras, Scikit-learn.

---

## ⚙️ Instalação

Para rodar este projeto localmente, siga os passos abaixo:

1.  **Clone o repositório:**
   
    ```bash
    git clone github.com/JaoMachado/VeritasAI-Deepfake-Detection.git
    cd VeritasAI-Deepfake-Detection
    ```

3.  **Crie um ambiente virtual e ative-o:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows, use `venv\Scripts\activate`
    ```

4.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```
