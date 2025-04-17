# Criando arquivo README.md com todo o conteúdo em Markdown
markdown_content = """# Filtros Sobel em NumPy (Correlação e Convolução)

Este repositório apresenta uma implementação **em Python puro** (com NumPy e OpenCV) dos filtros de Sobel horizontal, aplicando tanto a operação de **correlação** quanto de **convolução** passo a passo, sem recorrer a funções prontas de bibliotecas de processamento.

---

## Descrição

- Leitura da imagem em BGR via OpenCV  
- Conversão para RGB e depois para escala de cinza  
- Definição manual do kernel Sobel horizontal  
- Cálculo de **padding** (zero‑padding) para manter as dimensões originais  
- Laços aninhados que percorrem cada pixel da imagem:  
  - **Correlação**: \\( \\sum f(x+u,y+v)\\,w(u,v) \\)  
  - **Convolução**: \\( \\sum f(x+u,y+v)\\,w(-u,-v) \\)  
- Exibição dos resultados lado a lado com Matplotlib  

---

## Pré‑requisitos

- Python 3.x  
- NumPy  
- OpenCV (`cv2`)  
- Matplotlib  

Instale com:

```bash
pip install numpy opencv-python matplotlib
