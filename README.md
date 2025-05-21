# 🏍️ Detecção de Motos com YOLOv5 + OpenCV

Este projeto utiliza **visão computacional** com **YOLOv5** e **OpenCV** para detectar motos em um vídeo de forma automática e marcar aquelas que estão “prontas para uso” com um retângulo verde.

---
## 🔍 O que o código faz?
- Carrega um modelo YOLOv5 pré-treinado (yolov5s) para detectar objetos em tempo real.
- Abre um vídeo e processa frame a frame.
- Detecta motos (motorcycle) em cada frame.
- Desenha um retângulo verde em volta das motos detectadas e escreve o status da moto.
- Exibe o vídeo com as anotações.
---

## 🚀 Tecnologias Utilizadas

| Tecnologia | Descrição |
|------------|-----------|
| **Python 3** | Linguagem de programação usada no projeto. |
| **OpenCV** (`cv2`) | Biblioteca para manipulação de imagens e vídeos em tempo real. |
| **PyTorch** (`torch`) | Framework de machine learning usado para carregar o modelo YOLOv5. |
| **YOLOv5** | Modelo pré-treinado de detecção de objetos em tempo real. |
| **Ultralytics Hub** | Permite baixar modelos YOLOv5 diretamente via PyTorch Hub. |

---

## 📦 Requisitos

Antes de executar o projeto, você precisa ter:

- Python 3.7 ou superior instalado
- Pip atualizado

---

## 📥 Instalação

### 1. **Clone o repositório (ou salve o arquivo `.py`):**

```bash
git clone https://github.com/edu1805/Challenge-IoT.git
cd seu-repositorio
```
### 2. **Instale as dependências:**

```bash
pip install torch torchvision opencv-python
```
---

## 📹 Como usar

**Execute o script**
```bash
python detectar_motos.py
```
**🔴 Para encerrar o vídeo a qualquer momento, pressione a tecla Q.**
