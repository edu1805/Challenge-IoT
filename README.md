# 🏍️ Detecção de Motos com YOLOv5 + OpenCV

Este projeto utiliza **visão computacional** com **YOLOv5** e **OpenCV** para detectar motos em imagens e vídeos. O objetivo é organizar o pátio da empresa identificando o status de cada moto: **pronta para uso**, **em revisão**, **reservada**.

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
O projeto conta com **3 scripts principais**:
| Arquivo | Tipo de entrada | Finalidade |
|--------|------------------|------------|
| `detectar_motos_simples.py` | 🎥 Vídeo | Detecta motos e marca como “pronta” com retângulo verde |
| `detectar_motos_2.py` | 🎥 Vídeo | Detecta motos e marca como "em revisão" com retângulos amarelos |
| `detectar_imagens.py` | 🖼️ Imagem | Detecta motos em uma imagem estática e amarca como "reservada" com retângulos azuis |

Cada um pode ser usado separadamente dependendo da sua fonte de entrada e objetivo.

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
python detectar_motos_simples.py
```
para ver motos detectadas como "pronta";

**Execute o script**
```bash
python detectar_motos_2.py
```
para ver motos detectadas como "em revisão";

**Execute o script**
```bash
python detectar_imagens.py
```
para ver motos detectadas em uma imagem como "reservado".

### **🔴 Para encerrar o vídeo a qualquer momento, pressione a tecla Q.**
