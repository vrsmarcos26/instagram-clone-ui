<div align="center">
  <h1>
    Clone da Interface do Instagram (Feed)
  </h1>
</div>

<p align="center">
  <img alt="Tecnologia Principal" src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white">
  <img alt="Linguagem do Layout" src="https://img.shields.io/badge/XML-d9534f?style=for-the-badge&logo=android-studio&logoColor=white">
  <img alt="Licença" src="https://img.shields.io/github/license/vrsmarcos26/instagram-clone-ui?style=for-the-badge&color=blue">
</p>

<p align="center">
  Recriação da interface principal (feed) do Instagram utilizando XML e componentes nativos do Android Studio, como parte de um estudo sobre layouts complexos.
</p>

<p align="center">
  <a href="#-sobre-o-projeto">Sobre</a> •
  <a href="#-tecnologias-utilizadas">Tecnologias</a> •
  <a href="#-como-usar">Como Usar</a> •
  <a href="#-demonstração">Demonstração</a> •
  <a href="#-licença">Licença</a>
</p>

---

### 🎯 Sobre o Projeto

Este projeto é um exercício de desenvolvimento de interface de usuário (UI) para Android, focado em replicar a tela de feed do Instagram. O objetivo foi aprofundar os conhecimentos em layouts responsivos e na utilização de componentes como `ConstraintLayout`, `ScrollView` e `ImageView` para construir uma UI moderna e familiar. Este foi um trabalho desenvolvido para fins acadêmicos, agora aprimorado para compor meu portfólio.

---

### 🛠️ Tecnologias Utilizadas

A interface foi construída utilizando as ferramentas padrão do desenvolvimento Android nativo.

<p align="center">
  <a href="#"><img src="https://img.shields.io/badge/Android_Studio-3DDC84?style=for-the-badge&logo=android-studio&logoColor=white" alt="Android Studio"></a>
  <a href="#"><img src="https://img.shields.io/badge/XML-d9534f?style=for-the-badge&logo=android-studio&logoColor=white" alt="XML"></a>
  <a href="#"><img src="https://img.shields.io/badge/ConstraintLayout-448AFF?style=for-the-badge" alt="ConstraintLayout"></a>
</p>

---

### ⚙️ Como Usar

Para visualizar este layout:
1.  Crie um novo projeto no Android Studio.
2.  Copie o conteúdo do arquivo `instagram.xml` para o seu arquivo de layout principal (ex: `res/layout/activity_main.xml`).
3.  Na sua `MainActivity.kt` ou `MainActivity.java`, certifique-se de que o layout está sendo carregado: `setContentView(R.layout.activity_main)`.
4.  Execute o aplicativo em um emulador ou dispositivo físico.

---

### 🎬 Demonstração

**➡️ IMPORTANTE:** Substitua o link abaixo por um screenshot do seu app rodando!

arquivo print

<summary><strong>💡 Análise da Estrutura do Layout (Write-up)</strong></summary>
<br>

A estrutura deste layout foi pensada para espelhar a complexidade da tela do Instagram, dividindo a UI em componentes reutilizáveis e organizados:

1.  **Layout Raiz (`ConstraintLayout`)**: Escolhido como o contêiner principal para permitir o posicionamento flexível e relativo dos elementos, evitando o aninhamento excessivo de layouts (`layout nesting`).

2.  **Barra Superior (Header)**: Contém o logo "Instagram" e os ícones de ações (`ImageViews` para adicionar post, likes e mensagens), todos alinhados e restringidos (`constrained`) às bordas do `ConstraintLayout` pai.

3.  **Seção de Stories (`HorizontalScrollView`)**: Para a lista de stories, um `HorizontalScrollView` foi utilizado para permitir a rolagem horizontal. Dentro dele, um `LinearLayout` agrupa cada story individual, que por sua vez é um `LinearLayout` vertical contendo uma `ImageView` para a foto de perfil e um `TextView` para o nome do usuário.

4.  **Postagem do Feed**:
    -   O card de postagem é um `LinearLayout` vertical.
    -   O cabeçalho do post (foto, nome, localização) e o corpo (imagem principal) são posicionados de forma clara.
    -   A barra de ações (curtir, comentar, compartilhar, salvar) utiliza um `LinearLayout` horizontal com `ImageViews` distribuídos.
    -   Os textos de curtidas, descrição e comentários são `TextViews` estilizados para corresponder à aparência do app original.

5.  **Barra de Navegação Inferior (Bottom Bar)**: Um `LinearLayout` horizontal fixado na parte inferior da tela, contendo os ícones de navegação. O uso de `layout_weight` garante que os ícones se distribuam igualmente pelo espaço disponível.


---

### 📝 Licença

Este projeto está sob a licença MIT.

<hr>

<p align="center">
  Desenvolvido por <b>SEU NOME</b>
</p>
