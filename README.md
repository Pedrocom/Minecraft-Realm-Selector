# ⛏️ Minecraft Realm - Seletor de Profissões

Uma ferramenta web leve e interativa desenvolvida para organizar os papéis e especialidades dos membros num servidor de **Minecraft Realms**, com sincronização em tempo real.

---

##  Tecnologias Utilizadas

* **HTML5**
* **Tailwind CSS** (via CDN para um design moderno e responsivo)
* **Alpine.js** (para reatividade e lógica do frontend)
* **Supabase** (Base de dados em nuvem para sincronização em tempo real)

---

## Funcionalidades

* **Identificação de Jogador:** Insere o nick exato do Minecraft para gerir o papel.
* **Catálogo de Profissões:** Visualização de várias especialidades (Fazendeiro, Guerreiro, Arqueiro, Armeiro, Construtor, Redstoner, Explorador e Minerador).
* **Painel em Tempo Real:** Mostra instantaneamente quem já escolheu qual profissão no Realm.
* **Persistência de Dados:** Gravação automática na nuvem e salvamento do nick no `localStorage` do navegador.

---

## Estrutura da Base de Dados (Supabase)

A aplicação comunica com uma tabela chamada **`jogadores`** com a seguinte estrutura básica:

* `id`: Identificador único (número gerado)
* `nome`: `text` (Nick do jogador)
* `profissao`: `text` (Papel escolhido)

---

## 
Como Utilizar

1. Clone ou faça o download deste repositório.
2. Certifique-se de que tem uma tabela configurada no Supabase com o nome `jogadores`.
3. Insira as suas chaves do Supabase nas constantes `SUPABASE_URL` e `SUPABASE_KEY` dentro do código.
4. Abra o ficheiro `index.html` num navegador ou faça o deploy numa plataforma como o Netlify ou GitHub Pages.
