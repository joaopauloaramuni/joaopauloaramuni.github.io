-----

<img alt="githubpages" src="https://joaopauloaramuni.github.io/image/githubpages2.png?raw=true"/>

-----

# Repo GitHub Pages

## O que é o GitHub Pages? :octocat:

O **GitHub Pages** é um serviço gratuito oferecido pelo GitHub que permite que você hospede sites diretamente de um repositório. É amplamente utilizado para criar **portfólios, blogs, páginas de projetos** ou documentações de forma simples e integrada ao fluxo de versionamento.

Os sites do GitHub Pages podem ser gerados a partir de arquivos HTML estáticos ou usando geradores de site como o **Jekyll**, que é suportado nativamente.

- Endereço típico: `https://<usuário>.github.io/<repositório>/`
- Pode ser ativado nas configurações do repositório (Settings > Pages)
- Pode usar domínio personalizado

## 🧑‍💻 Por que usar o GitHub Pages para criar seu portfólio?

O **GitHub Pages** é uma excelente opção para desenvolvedores que desejam criar um site de currículo ou portfólio técnico, porque:

- ✅ É gratuito e fácil de configurar
- 🔗 Se integra diretamente com seu repositório GitHub
- 🧾 Permite publicar HTML, CSS e JS sem precisar de um servidor
- 🌐 Gera uma URL estável e profissional: `https://seunome.github.io/`
- 🖼️ Pode hospedar imagens, projetos, e exemplos de código

Você pode construir sua página manualmente com HTML/CSS ou usar templates prontos com **Jekyll**.

É uma forma prática de apresentar seus projetos, contatos e experiência diretamente a partir da plataforma onde você já colabora com código.

---

## Renderização de imagens no GitHub

### Como imagens são tratadas em repositórios comuns

Ao armazenar imagens diretamente em um repositório (por exemplo, dentro da pasta `/images`), o GitHub exibe os arquivos de imagem com uma URL voltada para **visualização e controle de versão**, e não para **uso público direto**. Isso significa que:

- As imagens são servidas com URLs longas, muitas vezes com tokens e hashes.
- Elas podem ser instáveis e mudarem a cada push ou alteração de commit.
- Não são otimizadas para uso em sites públicos (headers, cache, CDN).

### Por que hospedar imagens no GitHub Pages?

Quando você usa o GitHub Pages para hospedar imagens:

- As imagens são servidas como **conteúdo estático puro**, ideal para sites.
- Elas têm **URLs limpas e permanentes**, como:  
  `https://<usuário>.github.io/<repositório>/images/foto.png`
- São automaticamente servidas via **CDN do GitHub**, (Content Delivery Network - ou Rede de Distribuição de Conteúdo) com melhor desempenho.
- Isso evita problemas de links quebrados ou bloqueios por CORS.

📌 **Dica**: Crie uma pasta chamada `assets` ou `images` e coloque suas imagens lá. No HTML/Markdown, use:

```markdown
![Descrição da imagem](https://<usuário>.github.io/<repositório>/images/nome-da-imagem.png)
```

## 📦 O que é uma CDN?

CDN (**Content Delivery Network**) é uma rede de servidores distribuídos globalmente que entrega conteúdos da web de forma rápida e eficiente.

Quando você acessa um site ou arquivo hospedado em uma CDN, a resposta vem do servidor mais próximo da sua localização, garantindo menor latência, maior velocidade de carregamento e mais confiabilidade.

### ✅ Vantagens:

- 🚀 Carregamento mais rápido de arquivos estáticos (imagens, CSS, JS etc.)
- 🌍 Melhor desempenho global
- 📉 Redução de carga no servidor principal
- 🔐 Mais segurança contra ataques como DDoS
- 📦 Otimização de cache e entrega de conteúdo

O GitHub Pages usa uma CDN para distribuir os arquivos dos seus sites, o que melhora a performance significativamente — especialmente para imagens e recursos estáticos.

---

## Documentação e links úteis

### Documentação oficial
- [GitHub Pages - Documentação](https://docs.github.com/pt/pages)
- [Configurar um site com Jekyll](https://docs.github.com/pt/pages/setting-up-a-github-pages-site-with-jekyll)
- [GitHub Pages + Domínio personalizado](https://docs.github.com/pt/pages/configuring-a-custom-domain-for-your-github-pages-site)

### Tutoriais e recursos extras
- [Guia Completo do GitHub Pages (em inglês)](https://pages.github.com/)
- [Jekyll - Gerador de sites estáticos](https://jekyllrb.com/)
- [Markdown Cheatsheet](https://www.markdownguide.org/cheat-sheet/)
- [Exemplo de repositório com GitHub Pages](https://github.com/daattali/beautiful-jekyll)

### Exemplos de uso do GitHub Pages:
- [Comunidade Python-MG](https://pythonmg.github.io/)
- [Repositório com o conteúdo das disciplinas GPP e MDS do curso Engenharia de Software da Universidade de Brasília](https://fga-eps-mds.github.io/A-Disciplina-MDS-EPS/)

---

## Exemplo de estrutura de diretório

```
meu-site/
├── index.html
├── about.html
├── images/
│   └── foto-perfil.png
├── css/
│   └── estilo.css
└── CNAME  (opcional, para domínio próprio)
```

---

## Faça o teste

O GitHub Pages é uma solução prática, gratuita e poderosa para quem deseja criar um site estático com facilidade. E quando usado corretamente, pode inclusive funcionar como um **CDN gratuito para imagens e outros recursos estáticos**.

-----
