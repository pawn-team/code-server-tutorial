# code-server-tutorial
0️⃣0️⃣0️⃣2️⃣: Como instalar VS-Code no Termux

**OBS:** Método disponível apenas no Termux!

**1° Passo:** Instalar repositório externo
  - **Descrição:** Isto permite que outros repositórios compatíveis não incluídos estejam disponíveis para instalação.
  - **Comandos:** `pkg install -y tur-repo`

**2° Passo:** Instalar pacote code-server
  - **Descrição:** Code-Server é um binário criado especialmente para dispositivos arm, servindo como um lançador do Web VSCode.
  - **Comandos:** `pkg install -y code-server`

**3° Passo:** Configurar senha de acesso
  - **Descrição:** Por segurança, Web VSCode exige senha de usuário para que ninguém possa invadir seus arquivos, a senha fica na frente da palavra-chave "password"
  - **Comandos:** `nano ~/.config/code-server/config.yml`

**4° Passo:** Iniciar o Web VSCode
  - **Descrição:** Isto vai fazer com que o editor esteja disponível para uso, e tambem abrir o navegador direto na tela de login.
  - **Comandos:** `code-server & sleep 2 && termux-open-url https://127.0.0.1:8080`

Esse tutorial foi baseado em um video do gringo <a href="https://youtu.be/O-6V5aKe-jo?si=W3ZlvdbLSAWlv6Tt">Technolex</a>
