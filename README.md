# 🩸 Rede de Doação de Sangue

Aplicação móvel Android desenvolvida no âmbito da disciplina de **Computação Móvel**, com o objectivo de facilitar a ligação entre dadores de sangue e pessoas ou instituições que necessitam de transfusões em situações normais ou de emergência.

## 📖 Descrição

A disponibilidade de sangue é fundamental para cirurgias, tratamentos médicos e atendimento a emergências. Contudo, a procura por dadores compatíveis continua a ser um processo moroso e pouco eficiente.

A **Rede de Doação de Sangue** pretende criar uma plataforma centralizada que permita a criação de uma comunidade de dadores, facilitando a divulgação de pedidos de sangue e a localização de potenciais dadores compatíveis.

## 🎯 Objectivos

### Objectivo Geral

Desenvolver uma aplicação móvel Android que permita criar uma rede de dadores, facilitando a divulgação de pedidos de sangue e a localização de potenciais doadores.

### Objectivos Específicos

* Permitir o registo de utilizadores e dos respectivos grupos sanguíneos;
* Publicar pedidos de doação de sangue;
* Pesquisar dadores por grupo sanguíneo;
* Disponibilizar informações de contacto entre utilizadores;
* Enviar notificações em situações de emergência;
* Promover a cultura de doação voluntária.

## ✨ Funcionalidades Principais

* 🔐 Registo e autenticação de utilizadores;
* 👤 Criação e gestão do perfil do dador;
* 🩸 Pesquisa de dadores por grupo sanguíneo;
* 🚨 Publicação de pedidos urgentes de sangue;
* 🔔 Sistema de notificações;
* 📋 Histórico de doações realizadas.

## 🏗 Arquitectura

O projecto segue a arquitectura **MVVM (Model-View-ViewModel)**, promovendo uma melhor separação de responsabilidades, maior manutenibilidade e escalabilidade da aplicação.

```
UI (Jetpack Compose)
        ↓
ViewModel
        ↓
Repository
        ↓
Firebase Services
(Authentication + Firestore)
```

## 🛠 Tecnologias Utilizadas

* **Kotlin**
* **Jetpack Compose**
* **Material Design 3**
* **MVVM**
* **StateFlow**
* **Firebase Authentication**
* **Cloud Firestore**
* **Android Studio**

## 📂 Estrutura do Projecto

```
app/
├── data/
│   ├── model/
│   ├── repository/
│   └── remote/
├── ui/
│   ├── screens/
│   ├── components/
│   └── theme/
├── viewmodel/
├── navigation/
└── utils/
```

## 🚀 Impacto Esperado

Espera-se que esta aplicação contribua para:

* Reduzir o tempo necessário para encontrar dadores compatíveis;
* Melhorar a resposta em situações de emergência;
* Incentivar a prática da doação voluntária;
* Aproximar dadores, receptores e instituições de saúde;
* Contribuir positivamente para a saúde pública.

## 👥 Equipa de Desenvolvimento

Projecto desenvolvido por um grupo de **6 estudantes de Engenharia Informática**, no âmbito da disciplina de **Computação Móvel**.

| Membro | Função          |
| ------ | --------------- |
| Anwar Machado | Desenvolvimento |
| Melvin Chemane | Desenvolvimento |
| Shenil Gafuro | Desenvolvimento |
| Suely Buque | Desenvolvimento |
| Vlad Van | Desenvolvimento |
| Yunisse Langa | Desenvolvimento |

## 📚 Disciplina

**Computação Móvel**
Licenciatura em Engenharia Informática

---

> "Uma doação pode salvar várias vidas."


### Running the apps

Use the run configurations provided by the run widget in your IDE's toolbar. You can also use these commands and options:

- Android app: `./gradlew :androidApp:assembleDebug`
- Desktop app:
  - Hot reload: `./gradlew :desktopApp:hotRun --auto`
  - Standard run: `./gradlew :desktopApp:run`
- Web app:
  - Wasm target (faster, modern browsers): `./gradlew :webApp:wasmJsBrowserDevelopmentRun`
  - JS target (slower, supports older browsers): `./gradlew :webApp:jsBrowserDevelopmentRun`
- iOS app: open the [/iosApp](./iosApp) directory in Xcode and run it from there.

### Running tests

Use the run button in your IDE's editor gutter, or run tests using Gradle tasks:

- Android tests: `./gradlew :shared:testAndroidHostTest`
- Desktop tests: `./gradlew :shared:jvmTest`
- Web tests:
  - Wasm target: `./gradlew :shared:wasmJsTest`
  - JS target: `./gradlew :shared:jsTest`
- iOS tests: `./gradlew :shared:iosSimulatorArm64Test`

---

Learn more about [Kotlin Multiplatform](https://www.jetbrains.com/help/kotlin-multiplatform-dev/get-started.html),
[Compose Multiplatform](https://github.com/JetBrains/compose-multiplatform/#compose-multiplatform),
[Kotlin/Wasm](https://kotl.in/wasm/)…

We would appreciate your feedback on Compose/Web and Kotlin/Wasm in the public Slack channel [#compose-web](https://slack-chats.kotlinlang.org/c/compose-web).
If you face any issues, please report them on [YouTrack](https://youtrack.jetbrains.com/newIssue?project=CMP).
