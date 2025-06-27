# Oasis App 🌴

Bem-vindo ao Oasis, seu aplicativo de preparação para concursos e vestibulares! Este projeto foi desenvolvido com [Expo](https://expo.dev) e visa fornecer uma plataforma completa para estudantes, com materiais de estudo, questões, acompanhamento de progresso e muito mais.

## ✨ Funcionalidades Principais

*   **Autenticação de Usuário:** Crie sua conta e faça login para ter acesso personalizado.
*   **Conteúdo Educacional:**
    *   Aulas introdutórias para diferentes concursos (Correios, ENEM, etc.).
    *   Banco de questões com cartões interativos.
    *   Questões categorizadas por área do conhecimento (Exatas, Humanas, Linguagens, Natureza).
    *   Gabaritos para conferência.
*   **Perfil de Usuário:** Visualize e edite suas informações de perfil.
*   **Acompanhamento de Progresso:** Monitore seu desempenho e evolução nos estudos.
*   **Cursos e Provas:** Explore listas de cursos e provas disponíveis.
*   **Planos de Estudo:** Acesse planos de estudo direcionados para provas específicas (Correios, ENEM, USP, VUNESP).
*   **Interface Intuitiva:** Navegação fluida e amigável, com telas de splash e carregamento para uma melhor experiência.

## 🛠️ Tecnologias Utilizadas

*   **Framework:** [Expo](https://expo.dev) (~52.0.46)
*   **Linguagem:** JavaScript e [TypeScript](https://www.typescriptlang.org/) (^5.3.3)
*   **UI:** [React](https://reactjs.org/) (18.3.1), [React Native](https://reactnative.dev/) (0.76.9)
*   **Roteamento:** [Expo Router](https://docs.expo.dev/router/introduction/) (~4.0.21)
*   **Navegação:** [React Navigation (Bottom Tabs)](https://reactnavigation.org/) (^7.0.0)
*   **Requisições HTTP:** [Axios](https://axios-http.com/) (^1.10.0)
*   **Gerenciamento de Estado:** React Context API (ex: `ScrollContext`)
*   **Componentes UI:**
    *   [React Native Paper](https://callstack.github.io/react-native-paper/) (^5.13.1)
    *   [React Native Elements (RNEUI)](https://reactnativeelements.com/) (^4.0.0-rc.8)
    *   [Gorhom Bottom Sheet](https://gorhom.github.io/react-native-bottom-sheet/) (^5.1.2)
*   **Armazenamento Local:** [@react-native-async-storage/async-storage](https://react-native-async-storage.github.io/async-storage/) (^1.23.1)
*   **Recursos Adicionais:**
    *   Expo AV (Áudio/Vídeo)
    *   Expo Font (Fontes Customizadas)
    *   Expo Image Picker (Seleção de Imagens)
    *   Expo Linear Gradient (Gradientes)
    *   React Native Calendars
    *   React Native Chart Kit (Gráficos)
    *   React Native Gesture Handler & Reanimated (Animações e Gestos)
*   **Testes:** [Jest](https://jestjs.io/) e Jest Expo

## 📁 Estrutura de Pastas

```
.
├── app/                      # Telas e configuração de rotas (Expo Router)
│   ├── pages/                # Páginas da aplicação
│   │   ├── content/          # Telas de conteúdo (aulas, questões)
│   │   └── main/             # Telas principais (login, home, perfil, etc.)
│   ├── _layout.tsx           # Layout principal da aplicação
│   └── index.tsx             # Ponto de entrada da navegação
├── assets/                   # Recursos estáticos (fontes, imagens, vídeos)
│   ├── fonts/
│   └── images/
├── components/               # Componentes React reutilizáveis
├── contexts/                 # Contextos React para gerenciamento de estado global
├── data/                     # Dados mockados ou estáticos (ex: SliderData)
├── services/                 # Lógica de negócios e integrações
│   └── hooks/                # Hooks customizados (ex: useLogin, useRegister)
├── server/                   # (Opcional) Código do backend mock ou stubs
├── app-example/              # Código de exemplo do Expo (pode ser removido)
├── .gitignore
├── app.json                  # Configurações do projeto Expo
├── babel.config.js           # Configuração do Babel
├── package.json              # Dependências e scripts do projeto
├── tsconfig.json             # Configuração do TypeScript
└── README.md                 # Este arquivo :)
```

## 🚀 Comece a Desenvolver

Siga os passos abaixo para configurar e executar o projeto em seu ambiente local.

1.  **Clone o repositório (se ainda não o fez):**
    ```bash
    git clone (https://github.com/JoaoVictor809/Oasis_.git)
    cd Oasis_
    ```

2.  **Instale as dependências:**
    Certifique-se de ter o [Node.js](https://nodejs.org/) (LTS) e o [npm](https://www.npmjs.com/) instalados.
    ```bash
    npm install
    ```

3.  **Configure o Backend (se aplicável):**
    Este projeto utiliza um backend para autenticação em `http://localhost:3000`. Certifique-se de que o servidor backend esteja rodando antes de iniciar o aplicativo. Se você não tiver o backend configurado, as funcionalidades de login e registro não funcionarão como esperado.

4.  **Inicie o aplicativo:**
    Você pode executar o aplicativo em diferentes plataformas:

    *   **Web:**
        ```bash
        npm run web
        ```
    *   **Android:**
        ```bash
        npm run android
        ```
        (Requer um emulador Android configurado ou um dispositivo físico conectado)
    *   **iOS:**
        ```bash
        npm run ios
        ```
        (Requer um simulador iOS configurado ou um dispositivo físico conectado, e ambiente macOS)

    Na saída do terminal, você encontrará opções para abrir o aplicativo em:
    *   Um [build de desenvolvimento](https://docs.expo.dev/develop/development-builds/introduction/)
    *   Um [emulador Android](https://docs.expo.dev/workflow/android-studio-emulator/)
    *   Um [simulador iOS](https://docs.expo.dev/workflow/ios-simulator/)
    *   [Expo Go](https://expo.dev/go) (para uma experiência sandbox mais limitada)

## 🧪 Testes

Para executar os testes (se configurados):
```bash
npm run test
```

## 🤝 Contribuição

Contribuições são bem-vindas! Se você deseja contribuir para o projeto, por favor:

1.  Faça um fork do repositório.
2.  Crie uma nova branch para sua feature (`git checkout -b feature/nova-feature`).
3.  Faça commit de suas mudanças (`git commit -am 'Adiciona nova feature'`).
4.  Faça push para a branch (`git push origin feature/nova-feature`).
5.  Abra um Pull Request.

## 📄 Licença

Este projeto é distribuído sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes (se existir).

---

Desenvolvido com ❤️ pela equipe Oasis.
