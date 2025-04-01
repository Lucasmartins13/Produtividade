# Projeto: Detecção de Pessoas com YOLOv8 e Heatmap

## Descrição
Este projeto utiliza visão computacional para detectar e rastrear pessoas em um vídeo. O objetivo é identificar a movimentação das pessoas em um ambiente e gerar um heatmap que destaca as áreas mais frequentadas. Para isso, foi utilizado o modelo YOLOv8 treinado para detecção de pessoas, com inferência realizada em Python usando OpenCV.

## Funcionalidades
- 📌 Detecção de pessoas em um vídeo.
- 🔥 Geração de um heatmap acumulado sobre as detecções.
- 🚶‍♂️ Identifica se a pessoa está parada ou em movimento.
- 🏢 Classifica as detecções por áreas específicas do ambiente.
- 🎥 Salva um vídeo processado com os resultados.
- 📊 Gera gráficos de movimentação por área.

## Tecnologias Utilizadas
- 🐍 Python
- 🖼 OpenCV
- 🤖 YOLOv8 (Ultralytics)
- 🔢 NumPy
- 📈 Matplotlib

## Como Usar
### Requisitos
Certifique-se de ter instalado:
```bash
pip install ultralytics opencv-python numpy matplotlib
