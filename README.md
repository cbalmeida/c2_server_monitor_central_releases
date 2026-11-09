# C2 Server Monitor Central — instaladores

Instaladores do **C2 Server Monitor Central**, o aplicativo da C2 Tecnologia que acompanha em tempo real os
servidores monitorados pelos agentes. O código fica num repositório privado; aqui só ficam as versões para
download e o manifesto `latest.json`, que a central consulta para se atualizar sozinha.

O aplicativo exige login de operador da C2: sem ele não mostra dados de nenhum cliente.

## Instalar

Baixe a versão mais recente em **[Releases](../../releases/latest)**.

- **Windows (10/11, 64 bits):** baixe `C2ServerMonitor-<versão>-setup.exe` e execute. A instalação é por usuário
  (não pede administrador). Como o instalador não tem assinatura de código, o Windows pode mostrar
  "O Windows protegeu o computador": clique em **Mais informações › Executar assim mesmo**.
- **Android:** baixe `C2-Monitor-Central-<versão>-android.apk` no celular e abra. Se o Android pedir, permita
  **instalar apps desta fonte** (navegador ou gerenciador de arquivos) e toque em **Instalar**.
- **macOS:** por enquanto a instalação é manual (o pacote do macOS é distribuído à parte).

## Atualizações

A partir da 1.1.0 a central verifica sozinha se há versão nova (ao abrir e a cada 6 horas) e mostra o aviso
"Nova versão disponível". No Windows a atualização é feita com um clique; no Android o sistema pede a sua
confirmação. Quem tem a 1.0.0 instala a 1.1.0 à mão uma vez.

Cada pacote tem o SHA-256 publicado no `latest.json`; a central confere o arquivo antes de instalar.
