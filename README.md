# 🚀 API de Delivery com Machine Learning

## 📌 Sobre o Projeto

Este projeto consiste no desenvolvimento de uma API REST para gerenciamento de pedidos de delivery, utilizando **FastAPI**, **SQLite** e integração com **Machine Learning** para classificação automática de prioridade dos pedidos.

O sistema permite criar, listar, atualizar, buscar e deletar pedidos, além de aplicar um modelo de aprendizado de máquina para prever a prioridade com base no item solicitado.

---

## 🛠️ Tecnologias Utilizadas

* Python 3
* FastAPI
* SQLite
* SQLAlchemy
* Pydantic
* Scikit-learn

---

## ⚙️ Funcionalidades

* ✅ Criar pedido
* ✅ Listar pedidos
* ✅ Buscar pedido por ID
* ✅ Atualizar status do pedido
* ✅ Deletar pedido
* ✅ Classificação automática de prioridade (Machine Learning)

---

## 🧠 Machine Learning

O projeto utiliza um modelo de classificação baseado em **Naive Bayes**, implementado com a biblioteca Scikit-learn.

Foi criada uma **pipeline de Machine Learning**, responsável por:

* Vetorização do texto (item do pedido)
* Treinamento do modelo
* Previsão da prioridade

### Exemplo:

Entrada:

```json
{
  "item": "pizza grande"
}
```

Saída:

```json
"prioridade": "alta"
```

---

## 📂 Estrutura do Projeto

```
delivery_system/
│
├── main.py
├── models.py
├── schemas.py
├── database.py
├── ml_model.py
├── requirements.txt
└── README.md
```

---

## ▶️ Como Executar o Projeto

### 1. Clonar o repositório

```
git clone <url-do-repositorio>
cd delivery_system
```

### 2. Criar ambiente virtual

```
python -m venv venv
venv\Scripts\activate
```

### 3. Instalar dependências

```
pip install -r requirements.txt
```

### 4. Rodar o servidor

```
python -m uvicorn main:app --reload
```

---

## 🌐 Acessar

