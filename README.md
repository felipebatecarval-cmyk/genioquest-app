# GenioQuest Android

Aplicativo Android nativo em Kotlin que abre `https://genioquest.com.br` em uma WebView imersiva. JavaScript, DOM Storage e cookies estão habilitados. O app solicita permissões Android para câmera e microfone quando a página as pede e encaminha uploads ao seletor de arquivos do sistema.

## Gerar APK localmente

Requisitos: JDK 17 e Gradle 8.9. Na raiz do projeto, execute `gradle assembleRelease`. O APK sem assinatura fica em `app/build/outputs/apk/release/app-release-unsigned.apk`.

## GitHub Actions

Envie o projeto ao GitHub e crie uma tag `v1.0.0` para compilar e anexar o APK ao release correspondente. Também é possível iniciar manualmente o workflow pela aba Actions; nesse caso, o APK fica disponível como artefato da execução.

O APK gerado pelo workflow é unsigned. Para distribuição pela Play Store, configure assinatura de release com um keystore e secrets do GitHub.
