# 🚀 README: Meu Currículo Dev (VS Code Style)

E aí, tudo certo? ✌️

Se você caiu aqui, provavelmente tá vendo o código do meu currículo. Eu cansei daqueles templates de Word sem graça e resolvi codar o meu próprio, inspirado na interface que a gente olha o dia inteiro: o VS Code (com aquele tema Dark maneiro na lateral).

Mas ó, **aviso importante**: Isso aqui é um "Work In Progress" (WIP). 🚧
Ainda tô ajustando umas margens, decidindo se coloco mais projetos e polindo o texto. Então se ver algum erro de digitação ou algo fora do lugar, releva que a versão final tá vindo!

---

## 💻 O que tem debaixo do capô? (Stack & Tecnologias)

Eu quis fazer algo que fosse bonito no browser, mas que não quebrasse se o RH resolvesse imprimir. Olha o que eu usei:

1.  **HTML5 Semântico**: Estrutura limpa, usando tags como `<aside>`, `<main>`, `<section>` pra ficar organizado.
    
2.  **Tailwind CSS (via CDN)**:
    *   Eu não queria configurar Node.js ou rodar `npm install` só pra um currículo estático.
    *   Usei o script da CDN, então o navegador carrega os estilos na hora.
    *   Vantagem: Dá pra estilizar tudo com classes utilitárias (tipo `text-blue-400`, `flex`, `p-8`) direto no HTML.

3.  **CSS "Puro" (@media print)**: 
    *   Aqui tá a mágica. Se você der um CTRL+P, vai ver que a sidebar preta fica branca?
    *   Fiz isso pra economizar tinta de impressora e ficar legível no papel. Tem regras específicas (`page-break`) pra garantir que o texto não seja cortado no meio da página.

4.  **Fontes**:
    *   *JetBrains Mono*: Pra tudo que parece código, títulos e JSON.
    *   *Inter*: Pro texto corrido, pra leitura não ficar cansativa.

5.  **Font Awesome**: Pros ícones das redes sociais e contatos.

---

## 🛠️ Como usar esse modelo (Tutorial Rápido)

Curtiu o layout e quer adaptar pro seu perfil? Fica à vontade! O código é 100% editável. Segue o passo a passo:

### 1. Preparação
Você só precisa de um editor de texto (VS Code, Sublime, Notepad++) e um navegador. Não precisa instalar nada.

### 2. Editando as informações
O código tá comentado pra facilitar. Procure por essas áreas no HTML:

*   **Sua Foto**: Procure pela `div` com `bg-[url(...)]`. Você pode trocar a URL pela sua foto hospedada ou colocar uma tag `<img>` ali dentro.
*   **Dados Pessoais**: Dá um CTRL+F e busca por "Contato". Só substituir o texto dentro dos `<span>`.
*   **Skills (O JSON Visual)**: Tá na seção `Stack.json`. Eu usei cores diferentes pra cada tecnologia (ex: `text-yellow-200` pro JS). Se quiser mudar a cor, é só trocar a classe do Tailwind.
*   **Experiência**: Cada emprego é um bloco `<div>`. Pode copiar e colar o bloco inteiro pra adicionar mais experiências.

### 3. Personalizando as Cores
Se você não curte o azul do VS Code (`blue-500`):
*   Dê um "Find and Replace" no código.
*   Troque `text-blue-` ou `border-blue-` por outra cor do Tailwind, tipo `purple`, `emerald` ou `rose`.

### 4. Salvando e Exportando
*   Salve o arquivo como `.html`.
*   Abra no Chrome/Edge/Firefox.
*   Aperte `CTRL + P` (Imprimir) e selecione "Salvar como PDF".
*   *Dica*: Nas configurações de impressão, ative a opção "Gráficos de plano de fundo" se quiser que as cores das barras de progresso apareçam.

---

Feito com ☕ e <codigo/> por Leviton Carvalho.