<template>
  <div class="analytics-guide-container">
    <h1 class="title">Guia de estilo Analytics</h1>

    <section class="section section--colors">
      <h2 class="section__title">Cores</h2>
      <div class="section__content">

        <div class="subsection">
          <h3 class="subsection__title">Azul primário</h3>
          <div class="color-and-code-container">
            <div class="color-box" style="backgroundColor: #00afef;"></div>
            <ul class="code-colors">
              <li class="code-color__title">Códigos:</li>
              <li class="code-color"><code>#00afef</code></li>
              <li class="code-color"><code>rgb(0, 175, 239)</code></li>
              <li class="code-color"><code>hsl(196, 100%, 47%)</code></li>
            </ul>
          </div>
        </div>

        <div class="subsection subsection--blue-variables">
          <h3 class="subsection__title">Variações do azul primário</h3>
          <div>
            <p>Para utilizar variações do azul é recomendado aplicar opacidade de 75%, 50% ou 30% no azul primário.</p>
            <div class="colors-container">
              <div class="color-box" style="backgroundColor: #00afef;">100%</div>
              <div class="color-box" style="backgroundColor: rgba(0, 175, 239, .75);">75%</div>
              <div class="color-box" style="backgroundColor: rgba(0, 175, 239, .5);">50%</div>
              <div class="color-box" style="backgroundColor: rgba(0, 175, 239, .3);">30%</div>
            </div>
          </div>
        </div>

        <div class="subsection">
          <h3 class="subsection__title">Azul secundário</h3>
          <div>
             <div class="color-and-code-container">
              <div class="color-box" style="backgroundColor: #252642;"></div>
              <ul class="code-colors">
                <li class="code-color__title">Códigos:</li>
                <li class="code-color"><code>#252642</code></li>
                <li class="code-color"><code>rgb(37, 38, 65)</code></li>
                <li class="code-color"><code>hsl(238, 28%, 20%)</code></li>
              </ul>
            </div>
          </div>
        </div>

        <div class="subsection subsection--others-colors">
          <h3 class="subsection__title">Outras cores</h3>
          <p>Para a aplicação de outras cores é recomendada a paleta abaixo.</p>
          <div class="others-colors-container">
            <div class="color-and-code-container">
              <div class="color-box" style="backgroundColor: #107CA3;"></div>
              <ul class="code-colors">
                <li class="code-color__title">Códigos:</li>
                <li class="code-color"><code>#107CA3</code></li>
                <li class="code-color"><code>rgb(16, 123, 162)</code></li>
                <li class="code-color"><code>hsl(196, 82%, 35%)</code></li>
              </ul>
            </div>
            <div class="color-and-code-container">
              <div class="color-box" style="backgroundColor: #CE0063;"></div>
              <ul class="code-colors">
                <li class="code-color__title">Códigos:</li>
                <li class="code-color"><code>#CE0063</code></li>
                <li class="code-color"><code>rgb(206, 0, 99)</code></li>
                <li class="code-color"><code>hsl(331, 100%, 40%)</code></li>
              </ul>
            </div>
            <div class="color-and-code-container">
              <div class="color-box" style="backgroundColor: #A6A6A6;"></div>
              <ul class="code-colors">
                <li class="code-color__title">Códigos:</li>
                <li class="code-color"><code>#A6A6A6</code></li>
                <li class="code-color"><code>rgb(166, 166, 166)</code></li>
                <li class="code-color"><code>hsl(0, 0%, 65%)</code></li>
              </ul>
            </div>
            <div class="color-and-code-container">
              <div class="color-box" style="backgroundColor: #F07C00;"></div>
              <ul class="code-colors">
                <li class="code-color__title">Códigos:</li>
                <li class="code-color"><code>#F07C00</code></li>
                <li class="code-color"><code>rgb(240, 124, 0)</code></li>
                <li class="code-color"><code>hsl(31, 100%, 47%))</code></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="section section--tipografy">
      <h2 class="section__title">Tipografia</h2>
      <div class="section__content">
        <div class="subsection">
          <h3 class="subsection__title">Font-family</h3>
          <p>A fonte padrão é 'Open Sans'.</p>
          <pre><code>font-family: 'Open Sans', sans-serif;</code></pre>
        </div>

        <div class="subsection">
          <h3 class="subsection__title">Peso da fonte</h3>
          <p>Os títulos dos relatórios utilizam a versão 'light', já o texto padrão a versão regular. Outros pesos disponíveis estão listados abaixo.</p>
          <ul>
            <li style="fontWeight: 300;">Light: 300</li>
            <li style="fontWeight: 400;">Regular (padrão): 400</li>
            <li style="fontWeight: 700;">Bold: 700</li>
            <li style="fontWeight: 800;">ExtraBold: 800</li>
          </ul>
          <pre><code>font-weight: 400;</code></pre>
        </div>

        <div class="subsection">
          <h3 class="subsection__title">Tamanho da fonte</h3>
          <p>O tamanhos pré definidos estão listados abaixo, mas podem ser adicionados novos tamanhos, conforme necessidade.</p>
          <ul>
            <li style="font-size: 28px;">Título desktop: 28px</li>
            <li style="font-size: 25px;">Título mobile: 25px</li>
            <li style="font-size: 14px;">Texto padrão desktop: 14px</li>
            <li style="font-size: 11px;">Texto padrão mobile: 11px</li>
          </ul>
          <pre><code>font-size: 14px;</code></pre>
        </div>
      </div>
    </section>

    <section class="section section--libraries">
      <h2 class="section__title">Responsividade</h2>
        <div class="section__content">
          <div class="subsection">
          <p>A estrutura do layout é alterada em dois endpoints principais. A versão desktop possui o menu lateral fixo na esquerda, nas telas com mais de 1023px de largura. Já a versão mobile possui o menu no estilo 'hamburguer', nas telas com até 1023px de largura. Podem ser acrescentados outros endpoits conforme necessidade, desde que não interfira na estrutura principal do layout.</p>

          <p>Para definir novos end-poits usar media queries. Exemplo:</p>

          <pre><code>
            @media only screen and (max-width: 1023px) {
                  //estilo
              }
            </code></pre>
        </div>
      </div>
    </section>

    <section class="section section--libraries">
      <h2 class="section__title">Bibliotecas</h2>
      <div class="section__content">
        <div class="subsection">
          <h3 class="subsection__title">Element UI</h3>
          <a href="https://element.eleme.io/#/en-US" target="_blank">Documentação</a>
          <p>A biblioteca Element UI é utilizada na criação dos filtros e tabelas dos relatórios. Também possui diversos outros elementos que podem ser usados conforme necessidade.</p>
        </div>

        <div class="subsection">
          <h3 class="subsection__title">SweetAlert</h3>
          <a href="https://sweetalert.js.org/" target="_blank">Documentação</a>
          <p>A biblioteca SweetAlert é utilizada na criação de alertas animados.</p>
          <pre><code>
          this.$swal.fire({
            icon: "warning",
            html: 'Mensagem do alerta.',
            confirmButtonText: "Entendi",
            confirmButtonColor: "#409EFF",
          });
          </code></pre>
        </div>

        <div class="subsection">
          <h3 class="subsection__title">Chart JS</h3>
          <a href="https://www.chartjs.org/docs/" target="_blank">Documentação</a>
          <p>A biblioteca Chart JS é utilizada na criação de gráficos informativos.</p>
        </div>
      </div>
    </section>

    <section class="section">
      <h2 class="section__title">Relatórios</h2>
      <div class="section__content">

        <div class="subsection">
          <h3 class="subsection__title">Filtros</h3>
          
          <p>Os filtros que são utilizados em mais de um relatório estão componentizados e podem ser acessados na pasta '<code>src\components\filters</code>'. Os que são utilizados apenas em um relatório podem ser criados utilizando a biblioteca <a href="https://element.eleme.io/#/en-US" target="_blank">Element UI</a>.</p>
          <p>Sempre que possível devem possuir a mesma largura e o alinhamento deve ser à esquerda, na versão desktop, e centralizados, na versão mobile.</p>
          <p>Alguns filtros iniciam escondidos e só aparecem quando clicado o botão de expandir. Estes devem possuir uma transição animada.</p>

          <p>Exemplo na versão desktop:</p>
          <img src="../../../assets/filters-desktop.gif" alt="">

          <p>Exemplo na versão mobile:</p>
          <img src="../../../assets/filters-mobile.gif" alt="">
        </div>

        <div class="subsection">
          <h3 class="subsection__title">Tabelas</h3>
          <p>As tabelas devem ser criadas utilizando a biblioteca <a href="https://element.eleme.io/#/en-US" target="_blank">Element UI</a>, respeitando as cores definidas neste guia.</p>
          <p>Exemplo de tabela:</p>
          <img src="../../../assets/report-example.png" alt="">
        </div>
      </div>
    </section>

  </div>
</template>

<script>
export default {
    name: 'AnalyticsStyleGuide',
}
</script>

<style lang="scss" scoped>

.section {
  padding: 60px 0px 10px 0px;
  border-bottom: 1px solid rgba(156, 156, 156, 0.498);

  &:first-of-type{
    padding-top: 20px;
  }

  .subsection {
    padding: 0 40px 40px 40px;
    margin-bottom: 40px;
    border-bottom: 1px solid rgba(188, 188, 188, 0.498);

    &:last-child {
      border-bottom: none;
    }

    .subsection__title {
      margin-bottom: 10px;
    }
  }

  pre {
    background-color: rgb(254, 254, 254);
    padding: 34px 16px 32px 32px;
  }

  code {
      color: #919191;
      font-size: 14px;
    }
}

.section--colors {

  .color-and-code-container {
    display: flex;
    align-items: center;
    gap: 15px;

  }
  .color-box {
    width: 100px;
    height: 100px;
    border-radius: 10px;
    display: grid;
    place-items: center;
  }
    

  .subsection--blue-variables, .subsection--others-colors {
    .colors-container {
      display: flex;
      gap: 20px;
    }
  }
      
  .code-colors {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  .others-colors-container {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
}





</style>
