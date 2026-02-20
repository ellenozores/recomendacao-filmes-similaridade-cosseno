# 🎬 Sistema de Recomendação de Filmes

Projeto desenvolvido em Python utilizando TF-IDF e Similaridade de Cossenos para recomendar filmes com base em características textuais.

## 👩‍💻 Autoras
- Ellen Ozores
- Mel Yukari

---

## 📌 Objetivo

Desenvolver um sistema de recomendação baseado em conteúdo (Content-Based Filtering), utilizando informações como:

- Gêneros
- Diretores e elenco
- Descrição
- Tags

A recomendação é feita com base na Similaridade de Cossenos entre os vetores TF-IDF dos filmes.

---

## 🧠 Conceito Utilizado

### Similaridade de Cossenos

A Similaridade de Cossenos mede o ângulo entre dois vetores no espaço vetorial.

Fórmula:

cos(θ) = (A · B) / (||A|| ||B||)

Valores próximos de:
- 1 → Alta similaridade
- 0 → Sem similaridade
- -1 → Totalmente opostos

Neste projeto, a métrica foi aplicada utilizando:

- `TfidfVectorizer`
- `cosine_similarity`

Da biblioteca `scikit-learn`.

---

## Tecnologias Utilizadas

- Python
- NumPy
- Pandas
- NLTK
- Scikit-Learn

---

## 📊 Etapas do Algoritmo

1. Leitura dos datasets (Filmes, Dados e Tags)
2. Junção das tabelas
3. Criação da coluna "infos" contendo:
   - Gêneros
   - Diretores e elenco
   - Descrição
   - Tags
4. Limpeza do texto:
   - Conversão para minúsculo
   - Remoção de stopwords
5. Vetorização com TF-IDF
6. Cálculo da matriz de similaridade de cossenos
7. Retorno dos filmes mais similares ao escolhido pelo usuário

---

## ▶️ Como Executar
1. Baixe os arquivos .csv
2. Faça upload deles na plataforma usada para copilar o código
3. Execute os comandos
4. Digite o nome do filme EM INGLÊS e com as letras INICIAIS EM MAIÚSCULA

## 📌 Exemplo de Uso
Entrada: Toy Story
Saída: Toy Story 2, Monsters Inc, Finding Nemo...

