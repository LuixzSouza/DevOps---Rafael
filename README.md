# DevOps — Rafael

Repositório do exercício em grupo da disciplina de **DevOps**
(UNIVAS — Pouso Alegre/MG — Prof. Raffael Carvalho), referente à aula
*01 - Introdução ao DevOps: Controle de Versão e Colaboração*.

## Objetivo

Praticar o ciclo de colaboração com Git: `clone` → `branch` → `commit` →
`push` → **Pull Request** → `merge` → `pull`.

Todo o trabalho acontece no arquivo [`apresentacoes.md`](./apresentacoes.md):
cada integrante adiciona seu bloco de apresentação no final do arquivo, a partir
de uma branch com o seu primeiro nome.

## Papéis

| Papel | Quem | Responsabilidade |
| --- | --- | --- |
| Controlador | [@LuixzSouza](https://github.com/LuixzSouza) | Criou o repositório e é o **único** que faz o merge dos PRs |
| Integrantes | demais membros do grupo | Criam sua branch, fazem o commit/push e abrem o PR |

## Passo a passo — integrantes do grupo

1. **Clonar o repositório** (apenas na primeira vez):

   ```bash
   git clone https://github.com/LuixzSouza/DevOps---Rafael.git
   cd DevOps---Rafael
   ```

2. **Atualizar a base local:**

   ```bash
   git checkout main
   git pull origin main
   ```

3. **Criar a sua branch isolada** (use o seu primeiro nome):

   ```bash
   git checkout -b <seu-primeiro-nome>
   ```

4. **Implementar a mudança:** abra `apresentacoes.md` e adicione o seu bloco
   **no final do arquivo**, seguindo o modelo que está lá.

5. **Commit e push:**

   ```bash
   git add apresentacoes.md
   git commit -m "Adiciona apresentacao de <seu-nome>"
   git push origin <seu-primeiro-nome>
   ```

6. **Abrir o Pull Request:** no GitHub, abra um PR da sua branch para a `main`.

7. **Ver o resultado final** (depois que o PR for mesclado):

   ```bash
   git checkout main
   git pull origin main
   ```

## Passo a passo — responsável pelo merge

1. Aguardar os PRs dos colegas.
2. Revisar e fazer o **merge** de cada PR na `main` pela interface do GitHub.
3. Atualizar o repositório local:

   ```bash
   git pull origin main
   ```

## Regras de convivência

- Nunca faça commit direto na `main`; sempre passe por branch + PR.
- Adicione somente o **seu** bloco, sempre ao final do arquivo — assim os merges
  não geram conflito.
- Use mensagens de commit claras e descritivas.

## Material da aula

- [`01-Introdução ao DevOps.pdf`](./01-Introdução%20ao%20DevOps.pdf)
