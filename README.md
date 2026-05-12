# 🎬 Cinema Web

Aplicação web para visualizar filmes em cartaz no cinema, consumindo a API do TMDB.

## 💡 Ideia do Projeto

O usuário pode consultar os filmes atualmente em cartaz, marcar os que deseja assistir, registrar os que já assistiu, favoritar e dar uma nota pessoal.

## 🗂️ Classes do Domínio

### `Filme`

- id (TMDB)
- título
- sinopse
- nota
- poster

### `Genero`

- id
- nome

### `Usuario`

- id
- nome
- email
- senha

### `RegistroFilme`

- id
- status (quero ver / assistido / favorito)
- nota pessoal
- avaliação

## 🔗 Relações entre as Classes

| Relação                     | Tipo       |
| --------------------------- | ---------- |
| `Usuario` → `Filme`         | Associação |
| `Filme` → `Genero`          | Agregação  |
| `RegistroFilme` → `Usuario` | Composição |
| `RegistroFilme` → `Filme`   | Composição |
