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
```

### Preparação
1. Tenha o modelo YOLOv8 treinado salvo como `best (6).pt`.
2. Coloque o vídeo a ser processado na mesma pasta do código e nomeie-o como `70027081.mp4`.

### Execução
Para processar o vídeo, gerar os gráficos e visualizar os resultados, execute:
```bash
python codigo1.py
python codigo2.py
```
Os gráficos gerados serão salvos no diretório do projeto.

## Saída do Programa
Se o modelo detectar corretamente as pessoas, a saída incluirá:
- ✅ Um vídeo processado com as detecções e heatmap aplicado.
- 📊 Gráficos de movimentação e parada por área.
- 🔴 Destacação das pessoas paradas em vermelho e das em movimento em verde.

## Estrutura do Código
O código é dividido nas seguintes partes:
1. **Importação de bibliotecas**
   - OpenCV, NumPy, YOLOv8 e Matplotlib.
2. **Carregamento do modelo YOLOv8**
   - O modelo `best (6).pt` é carregado para detecção.
3. **Inicialização do processamento de vídeo**
   - O vídeo `70027081.mp4` é aberto com OpenCV.
   - Configuração do tamanho do frame e saída do vídeo processado.
4. **Loop principal (processamento frame a frame)**
   - Detecção de pessoas em cada frame.
   - Análise de movimentação e aplicação do heatmap.
   - Classificação das detecções por áreas do ambiente.
   - Exibição e salvamento do vídeo processado.
5. **Finalização**
   - Geração e salvamento dos gráficos.
   - Liberação dos recursos de vídeo.

## Possíveis Melhorias
Para obter melhores resultados, algumas melhorias podem ser implementadas:
- 📷 Utilização de um vídeo de maior qualidade para aumentar a precisão das detecções.
- 🚧 Captura do vídeo em uma área com menos objetos bloqueando as pessoas, evitando detecções incorretas.
- 🧠 Implementação de um sistema para identificar o que cada pessoa está fazendo, permitindo aplicações mais avançadas, como análise de comportamento e monitoramento de fluxo de clientes em estabelecimentos.

## Autor
Projeto desenvolvido utilizando YOLOv8 para visão computacional e análise de movimentação de pessoas em ambientes fechados.


